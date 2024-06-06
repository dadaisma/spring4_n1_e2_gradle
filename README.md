Spring and Gradle exercise



Access the page ->https://start.spring.io/, and generate a Spring boot project with the following characteristics:

PROJECT (dependency manager)

Gradle.

LANGUAGE

Java.

SPRING BOOT

The latest stable version.

PROJECT METADATA

Group

cat.itacademy.barcelonactiva.surnames.name.s04.t01.n02

artifact

S04T01N02GognomesName

Name

S04T01N02SurnamesName

Description

S04T01N02GognomesName

Package name

cat.itacademy.barcelonactiva.surnames.name.s04.t01.n02

PACKAGING

Jar

JAVA

Minimum version 11 

Dependencies:

Spring Boot DevTools

Spring Web


In the application.properties file, set the server.port variable to 9001.


We'll turn this app into a REST API:
Depending on the main package, create another subpackage called Controllers, and inside it, add the HelloWorldController class.

It should have two methods:

String greets
String greets2


These two methods will receive a String parameter called "name" and return the phrase:

“Hello, “ + name + “. You are running a Gradle project”.

The first method will respond to a GET request, and must be configured to receive the parameter as a RequestParam. The "name" parameter will have the default value "UNKNOWN".

You will have to answer to:

http://localhost:9001/HelloWorld
http://localhost:9001/HelloWorld?name=My name
 

The second method will respond to a GET request, and must be configured to receive the parameter as a PathVariable. The "name" parameter will be optional.

You will have to answer to:

http://localhost:9001/HelloWorld2
http://localhost:9001/HelloWorld2/myname


Useful links:
RequestParam:

->https://www.baeldung.com/spring-request-param


PathVariable:

->https://www.baeldung.com/spring-optional-path-variables


Diferències RequestParam i PathVariable:

->https://www.baeldung.com/spring-requestparam-vs-pathvariable


Diferències entre Maven i Gradle

->https://www.chakray.com/es/gradle-vs-maven-definiciones-diferencias/ ->https://programmerclick.com/article/47131530173/
