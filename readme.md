# Number Generator

Number Generator is a Jakarta-EE application that generates pseudo-random numbers and exposes a REST API.

## Pre-requisites

Before trying to run the application, ensure that you have met the following requirements:

### Java 8

Open your terminal and execute the following command to verify your Java version.

```
#java -version
openjdk version "1.8.0_232"
OpenJDK Runtime Environment (AdoptOpenJDK)(build 1.8.0_232-b09)
OpenJDK 64-Bit Server VM (AdoptOpenJDK)(build 25.232-b09, mixed mode)
```

### Apache Maven

Type the following command to verify if Apache Maven is working.
```
#mvn -v
Maven home: /Users/inerciobelton/Downloads/apache-maven-3.6.3
Java version: 1.8.0_102, vendor: Oracle Corporation, runtime: /Library/Java/JavaVirtualMachines/jdk1.8.0_102.jdk/Contents/Home/jre
Default locale: en_US, platform encoding: UTF-8
OS name: "mac os x", version: "10.12.6", arch: "x86_64", family: "mac"
```

### Jakarta EE 8 Application Server

Access the link [Jakarta EE Compatible Products](https://jakarta.ee/compatibility/) to see a full list of application servers that are compatible with the Jakarta EE 8 specification, including:

* [Wildfly 19.1.0](https://wildfly.org/downloads/)
* [Glassfish v5.1.0](https://projects.eclipse.org/projects/ee4j.glassfish/downloads)
* [OpenLiberty 19.0.0.9](https://openliberty.io/downloads/)


## Installation

To install the application locally, follow these steps:

Check out the source code to your computer:
```
git clone https://github.com/InercioBelton/number-generator.git
```
Navigate to the project directory and run the following command to build a clean package locally:
```
mvn clean install -P wildfly-managed

```
Note: The maven profile -Pwildfly-managed will start a new WildFly instance, and execute the tests, shutting it down when done. Make sure your application server is not running at this time to avoid confliting ports or adresses.
If you want to skip the tests execute the following command:
```
mvn clean install -P wildfly-managed -DskipTests

```

When the build is finished deploy the generated artifact to your favourite application server or use the DockerFile (at project root directory) to package the application in a Docker image.


## Usage

This application exposes a Rest API than can be accessed through the following endpoints:
 
* `POST /random`: [requests a new random number generation](/docs/random.md)
* `GET /history`: [get list of generated random numbers](/docs/history.md)
* `PUT /{requestId}/cancel`: [cancels a random number request](/docs/cancel.md)
* `GET stats`: [get system usage statistics](/docs/stats.md)
* `GET /pending`: [get the list of pending requests](/docs/pending.md)
* `PUT /threads`: [changes the size of the thread-pool](/docs/threads.md)
* `PUT /minRequestDuration`: [changes the minumum request duration](/docs/requestDuration.md)



