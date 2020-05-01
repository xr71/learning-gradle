# Projects

We can run multiple tasks, such as 
```
gradle clean build
gradle -i clean build
```


We can configure the build with source sets
```Gradle
sourceSets {
    main {
        java {
            srcDir 'src'
        }
    }

    test {

    }
}
```


The application plugin derives from the java plugin, can import just application.
To make use of application plugin `run`, make sure to specify the `mainClassName`


### To configure the specific jdk
```Gradle
java {
    sourceCompatibility = JavaVersion.VERSION_1_8
    targetCompatibility = ...
}
```


Can also use the java plugin to generate javadoc


We can use the same groovy or kts language for building kotlin files
