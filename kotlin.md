# Kotlin Programming Language

1. [Introduction](kotlin.md#introduction)
2. [References](kotlin.md#references)
3. [Tutorials](kotlin.md#tutorials)
4. [Samples](kotlin.md#samples)
5. [Should you switch from Java to Kotlin?](kotlin.md#should-you-switch-from-java-to-kotlin)
6. [Comparison to Java Programming Language](kotlin.md#comparison-to-java-programming-language)

## Introduction

"Kotlin is a statically typed programming language that runs on the Java virtual machine and also can be compiled to JavaScript source code or use the LLVM compiler infrastructure. Its primary development is from a team of JetBrains programmers based in Saint Petersburg, Russia.While the syntax is not compatible with Java, the JVM implementation of the Kotlin standard library is designed to interoperate with Java code and is reliant on Java code from the existing Java Class Library, such as the collections framework. Kotlin uses aggressive type inference to determine the type of values and expressions for which type has been left unstated. This reduces language verbosity relative to Java, which demands often entirely redundant type specifications prior to version 10.

As of Android Studio 3.0 \(released in October 2017\), Kotlin is fully supported by Google for use with their Android operating system, and is directly included in the IDE's installation package as an alternative to the standard Java compiler. The Android Kotlin compiler lets the user choose between targeting Java 6, Java 7, or Java 8-compatible bytecode."

[https://en.wikipedia.org/wiki/Kotlin\_\(programming\_language](https://en.wikipedia.org/wiki/Kotlin_%28programming_language)\)

## References

* [https://kotlinlang.org/](https://kotlinlang.org/)
* [https://kotlin.link/](https://kotlin.link/)
* [https://github.com/KotlinBy/awesome-kotlin](https://github.com/KotlinBy/awesome-kotlin)
* [https://kotlinlang.org/docs/reference/server-overview.html](https://kotlinlang.org/docs/reference/server-overview.html)
* [https://kotlinlang.org/docs/reference/comparison-to-java.html](https://kotlinlang.org/docs/reference/comparison-to-java.html)
* [https://kotlinlang.org/docs/books.html](https://kotlinlang.org/docs/books.html) books
* [https://github.com/KotlinBy/awesome-kotlin](https://github.com/KotlinBy/awesome-kotlin)
* [https://blog.gradle.org/kotlin-scripting-update](https://blog.gradle.org/kotlin-scripting-update)
* [https://codebeat.co/open-source/kotlin](https://codebeat.co/open-source/kotlin) - static code analysis
* [https://spring.io/blog/2017/01/04/introducing-kotlin-support-in-spring-framework-5-0](https://spring.io/blog/2017/01/04/introducing-kotlin-support-in-spring-framework-5-0)
* [https://kotlinlang.org/docs/reference/native-overview.html](https://kotlinlang.org/docs/reference/native-overview.html) kotlin native
* KotlinConf 2017 [https://www.youtube.com/playlist?list=PLQ176FUIyIUY6UK1cgVsbdPYA3X5WLam5](https://www.youtube.com/playlist?list=PLQ176FUIyIUY6UK1cgVsbdPYA3X5WLam5)
* [https://kotlinlang.org/docs/resources.html](https://kotlinlang.org/docs/resources.html)
* [http://www.baeldung.com/junit-5-kotlin](http://www.baeldung.com/junit-5-kotlin)
* [https://geek.justjoin.it/kotlin-coroutine-pewno-kolejny-krok-dla-programisty-rxjava/](https://geek.justjoin.it/kotlin-coroutine-pewno-kolejny-krok-dla-programisty-rxjava/) \(polish\)

## Tutorials:

* [https://try.kotlinlang.org/](https://try.kotlinlang.org/)
* [http://www.baeldung.com/spring-boot-kotlin](http://www.baeldung.com/spring-boot-kotlin)
* [https://fabiomsr.github.io/from-java-to-kotlin/](https://fabiomsr.github.io/from-java-to-kotlin/)
* [https://github.com/MindorksOpenSource/from-java-to-kotlin](https://github.com/MindorksOpenSource/from-java-to-kotlin)
* [https://engineering.talkdesk.com/migrating-from-java-to-kotlin-the-easy-way-37b25a379d72](https://engineering.talkdesk.com/migrating-from-java-to-kotlin-the-easy-way-37b25a379d72)
* [https://stackoverflow.com/questions/40499452/how-to-build-google-protocol-buffers-and-kotlin-using-gradle](https://stackoverflow.com/questions/40499452/how-to-build-google-protocol-buffers-and-kotlin-using-gradle)

## Samples:

* [https://github.com/ssouris/petclinic-spring5-reactive](https://github.com/ssouris/petclinic-spring5-reactive)
* [https://github.com/spring-petclinic/spring-petclinic-kotlin](https://github.com/spring-petclinic/spring-petclinic-kotlin)
* [https://github.com/FlavioF/kotlin-grpc-sample](https://github.com/FlavioF/kotlin-grpc-sample)
* [https://github.com/kgoralski/kotlin-springboot-template](https://github.com/kgoralski/kotlin-springboot-template)
* [https://github.com/kgoralski/kotlin-reactive-playground](https://github.com/kgoralski/kotlin-reactive-playground)
* [https://github.com/kgoralski/go-kotlin-java-kafka](https://github.com/kgoralski/go-kotlin-java-kafka)

## Should you switch from Java to Kotlin?

### Pros:

* "Better Java" & "Java after Effective Java" 
* Syntax Sugar
* Null safety & Immutability
* Easy to pick up by Java devs
* Spring Framework official support \(and this support is much better than year ago\)
* Google Android Support and Google using it too
* Data classes vs Lombok
* Great IDE support - Intellij can convert Java to Kotlin - but you can use Kotlin with Vim, VSCode and others... but IntelliJ recommended
* "when" pattern matching
* less boilerplate
* Maybe some devs with Kotlin will be better and more modern \(?\) - it would be good to create job ad with Kotlin and check feedback
* Java Interoperability
* Destructuring Declarations
* It is possible to mix Kotlin & Java in same project
* backed by Jetbrains
* Gradle Kotlin Script \(?\)
* Played with it and it is nice, also got some colleagues which are using it at their work and they like it
* Coroutines? [https://kotlinlang.org/docs/reference/coroutines.html](https://kotlinlang.org/docs/reference/coroutines.html)
* Kotlin Native? \(mobile\) [https://kotlinlang.org/docs/reference/native-overview.html](https://kotlinlang.org/docs/reference/native-overview.html)
* Got test libraries like Spek, KotlinTest... but you can use Spock or JUnit too
* it is polish ketchup [https://ketchupy.pl/](https://ketchupy.pl/) ;\)

### Cons:

* Most people will stick to Java
* Java development will be slower but it will probably catch Kotlin features later. But switching back to Java will be easy.
* "Better Java" - but still you need to learn it.
* Mindset change \(which is actually a pro to me\) - about null safety and immutability - using Kotlin as java is kinda ugly
* Switching from Kotlin to Java and from Java to Kotlin in multiple project is a little bit annoying
* Less tools? Like static code analysis? Still there are detekt, ktlint and plugin for SonarQube or codebeat.com
* Some compatibility Java problems
* Still it is a some kind of risk and time investment
* A litle bit slower compilation time \(?\)

### More opinnions:

* [https://medium.com/@magnus.chatt/why-you-should-totally-switch-to-kotlin-c7bbde9e10d5](https://medium.com/@magnus.chatt/why-you-should-totally-switch-to-kotlin-c7bbde9e10d5)
* [https://hashnode.com/post/why-i-abandoned-java-in-favour-of-kotlin-ciuzhmecf09khdc530m1ghu6d](https://hashnode.com/post/why-i-abandoned-java-in-favour-of-kotlin-ciuzhmecf09khdc530m1ghu6d)
* [http://natpryce.com/articles/000815.html](http://natpryce.com/articles/000815.html)
* [https://medium.com/keepsafe-engineering/kotlin-the-good-the-bad-and-the-ugly-bf5f09b87e6f](https://medium.com/keepsafe-engineering/kotlin-the-good-the-bad-and-the-ugly-bf5f09b87e6f)
* [https://www.quora.com/Would-you-use-Kotlin-to-build-back-end-microservices-Why-or-why-not](https://www.quora.com/Would-you-use-Kotlin-to-build-back-end-microservices-Why-or-why-not)
* [https://hackernoon.com/kotlin-in-production-should-you-stay-or-should-you-go-a3428b44b236](https://hackernoon.com/kotlin-in-production-should-you-stay-or-should-you-go-a3428b44b236)
* [https://medium.com/@Pinterest\_Engineering/the-case-against-kotlin-2c574cb87953](https://medium.com/@Pinterest_Engineering/the-case-against-kotlin-2c574cb87953)
* [https://medium.com/@mumayank/why-you-should-totally-switch-to-kotlin-not-3d20290d18bd](https://medium.com/@mumayank/why-you-should-totally-switch-to-kotlin-not-3d20290d18bd)
* [https://www.reddit.com/r/androiddev/comments/47613n/can\_we\_talk\_about\_the\_downsides\_of\_using\_kotlin/](https://www.reddit.com/r/androiddev/comments/47613n/can_we_talk_about_the_downsides_of_using_kotlin/)
* [https://medium.com/@xzan/the-drawbacks-of-migrating-to-kotlin-51f49a96107a](https://medium.com/@xzan/the-drawbacks-of-migrating-to-kotlin-51f49a96107a)

Also... new things in Java 10 [https://www.quora.com/What-is-new-in-Java-10/answer/Nick-Maiorano](https://www.quora.com/What-is-new-in-Java-10/answer/Nick-Maiorano)

## Comparison to Java Programming Language

[https://kotlinlang.org/docs/reference/comparison-to-java.html](https://kotlinlang.org/docs/reference/comparison-to-java.html)

"Some Java issues addressed in Kotlin

### Kotlin fixes a series of issues that Java suffers from:

* Null references are controlled by the type system.
* No raw types
* Arrays in Kotlin are invariant
* Kotlin has proper function types, as opposed to Java's SAM-conversions
* Use-site variance without wildcards
* Kotlin does not have checked exceptions

  **What Java has that Kotlin does not**

* Checked exceptions
* Primitive types that are not classes
* Static members
* Non-private fields
* Wildcard-types
* Ternary-operator a ? b : c

### What Kotlin has that Java does not

* Lambda expressions + Inline functions = performant custom control structures
* Extension functions
* Null-safety
* Smart casts
* String templates
* Properties
* Primary constructors
* First-class delegation
* Type inference for variable and property types
* Singletons
* Declaration-site variance & Type projections
* Range expressions
* Operator overloading
* Companion objects
* Data classes
* Separate interfaces for read-only and mutable collections
* Coroutines"

