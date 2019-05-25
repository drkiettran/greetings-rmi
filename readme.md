# greetings-rmi Remote Method Invocation with Java

Sample project using Java RMI messaging.

## Build

``` bash
mvn clean package
```

## Runs

### Run rmiregistry

```bash

export CLASSPATH=$CLASSPATH:target/greetings-rmi-1.0-SNAPSHOT-jar-with-dependencies.jar

rmiregistry

```

### Run Server

```bash
java -jar target/greetings-rmi-1.0-SNAPSHOT-jar-with-dependencies.jar server //student-VirtualBox/GreetingsServer
```

### Run Client

```bash

java -jar target/greetings-rmi-1.0-SNAPSHOT-jar-with-dependencies.jar client //student-VirtualBox/GreetingsServer "Johnny B Good"

```
