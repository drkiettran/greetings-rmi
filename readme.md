# greetings-rmi Remote Method Invocation with Java

Sample project using Java RMI messaging.
Updated with more specific instructions to run the app.
This program can act as a server or a client but not both.
The program arguments are to determine that role.

## Build

``` bash
mvn clean package
```

## Runs

### Run rmiregistry
Go to the folder of the project. Run the following comamnds:

```bash

export CLASSPATH=$CLASSPATH:target/greetings-rmi-1.0-SNAPSHOT-jar-with-dependencies.jar

rmiregistry

```

rmiregistry is a go between client server. It is a service broker that knows about
the functions of the server. It helps connect client to the server to interact to 
exchange data.

### Run Server

```bash

java -cp target/greetings-rmi-1.0-SNAPSHOT-jar-with-dependencies.jar edu.harrisburgu.cisc525.app.Main server //student-VirtualBox/GreetingServer
```

### Run Client

```bash

java -cp target/greetings-rmi-1.0-SNAPSHOT-jar-with-dependencies.jar edu.harrisburgu.cisc525.app.Main client //student-VirtualBox/GreetingsServer "Johnny B Good"

```
