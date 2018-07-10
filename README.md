# Create-react-app Maven WAR file example

Example of a [Create-react-app](https://github.com/facebook/create-react-app) build with [Maven](https://maven.apache.org/index.html) and deployed as WAR file to a [Docker Wildfly server](https://hub.docker.com/r/jboss/wildfly/).

## Prepare

```bash
npm install
```

## Build

```bash
mvn clean package
```

## Run

```bash
docker run -it -p 8080:8080 -v $PWD/deployments/:/opt/jboss/wildfly/standalone/deployments/ jboss/wildfly
```

You can now access your Create-react-app on [http://localhost:8080/](http://localhost:8080/create-react-app-example-1.0-SNAPSHOT/index.html).

