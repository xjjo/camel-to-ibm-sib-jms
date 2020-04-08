# objetivo
Integrar camel con ibm commerce a traves de sib.
- camel as consumer. (alimenta una ruta)
- camel as producer. (envia msg a was)

# Jars necesarios provistos por ibm  
disponibles en carpeta lib
1. com.ibm.ws.orb_7.0.0.jar
2. com.ibm.ws.sib.client.thin.jms_7.0.0.jar
3. com.ibm.ws.ejb.thinclient_7.0.0.jar

Agregarlos al repositorio local de Maven con los siguientes cmd:

```
mvn install:install-file -Dfile=C:\IBM\lib\com.ibm.ws.sib.client.thin.jms.jar -DgroupId=com.ibm -DartifactId=com.ibm.ws.sib.client.thin.jms -Dversion=7.0.0 -Dpackaging=jar

mvn install:install-file -Dfile=C:\IBM\lib\com.ibm.ws.ejb.thinclient.jar -DgroupId=com.ibm -DartifactId=com.ibm.ws.ejb.thinclient -Dversion=7.0.0 -Dpackaging=jar

mvn install:install-file -Dfile=C:\IBM\lib\com.ibm.ws.orb.jar -DgroupId=com.ibm -DartifactId=com.ibm.ws.orb -Dversion=7.0.0 -Dpackaging=jar
```

# run 
mvn camel:run


