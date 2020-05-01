# We have dependencies on:

* other projects
* external libraries
* internal libraries

Dependencies themselves have transitive dependencies

We can see these with:

```Bash
gradle -q dependencies
```

### Configuration scopes:

* implementation
  * compileOnly
  * runtimeOnly

* testImplementation
  * testCompileOnly
  * testRuntimeOnly

We can also satisfy repositories with:

* remote repo
* local file system


For local file:

```Gradle
repositories {
    flatDir {
        dir 'lib'
    }
}
```

For remote repo:

```Gradle
repositories {
    mavenCentral()
}

repositories {
    jcenter()
}
```

```Gradle
repositories {
    maven {
        url ""
    }

    ivy {
        url ""
    }
}
```