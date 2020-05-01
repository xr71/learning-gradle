# Gradle for Tests

Test Source Set:

* default `src/test/java`
* outputs to `build/classes/test`
* reports to `build/reports/test`

### Test Implementation Scope

```
dependencies {
    testImplementation 'junit:junit:4.12'
}
```

Make use of a test plugin

```Gradle
id 'com.adarshr.test-logger' version '2.0.0
```

From here, you can add options to the testlogger object:

```Gradle
testlogger {
    theme 'standard'
    showExceptions true
    ...
}

```