# Wrapper

We can ensure build consistency
By specifying the exact version of gradle to build with


init with
```
gradle wrapper
```

This will place a local gradle script in the directory
Can execute with

```Bash
./gradlew
```

This will generate a `gradle/wrapper/gradle-wrapper.properties` where you can set up the exact version

This will be very useful for continuous integration
We can use a build server like `teamcity`

