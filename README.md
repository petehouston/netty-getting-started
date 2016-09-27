# netty-getting-started

If you don't know where to start with Java/Netty, this tutorial is for you.

## Prerequisite

You need to prepare your environment:

* Java Development Kit (JDK 7 is preferrable for Netty 4)
* Gradle 3+
* A terminal

## Getting started

1. Init the project

```
$ gradle init --type java-library
```

2. Modify the `build.gradle`

```
apply plugin: 'java'
apply plugin: 'application'

mainClassName = 'com.petehouston.netty.tutorials.Main'

repositories {
    mavenCentral()
}

dependencies {
    compile 'io.netty:netty-all:4.1.5.Final'
}
```

The bootstrap class, which contains `main()` method to execute, is defined in `mainClassName`. You can update to your preference.

3. Update the `src` structure

```
└── src
    └── main
        └── java
            └── com
                └── petehouston
                    └── netty
                        └── tutorials
                            └── Main.java
```

4. The `Main.java` should contain a `main()` method.

5. To build project

```
$ gradle build
```

6. To execute project

```
$ gradle run
```

You can make it stop output unnecessary text by adding the quite mode `-q`:

```
$ gradle run -q
```

7. It is basically done for a Java/Netty project with Gradle. You can start writing Netty code from now.

