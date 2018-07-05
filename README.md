# Create-react-app Maven example to create a war file

Example of a create-react-app deployed to a wildfly server.

## Run

```bash
mvn clean install

docker run -it -p 8080:8080 -v $PWD/deployments/:/opt/jboss/wildfly/standalone/deployments/ jboss/wildfly
```

