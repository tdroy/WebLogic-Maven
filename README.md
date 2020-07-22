This is a demo project for WebLogic Maven plug-in.

Purpose is to compile & build a project, create new WLS domain, start servers, deploy project to domain.

First, WebLogic plugin required to install on maven repository. Here are the steps to install WLS maven plugin.

```
    Change directory to ORACLE_HOME\oracle_common\plugins\maven\com\oracle\maven\oracle-maven-sync\12.1.2.

    mvn install:install-file -DpomFile=oracle-maven-sync.12.1.2.pom -Dfile=oracle-maven-sync.12.1.2.jar.

    mvn com.oracle.maven:oracle-maven-sync:push -Doracle-maven-sync.oracleHome=c:\oracle\middleware\oracle_home\.

```

Once done, you can verify using below command.
```
mvn help:describe -DgroupId=com.oracle.weblogic -DartifactId=weblogic-maven-plugin -Dversion=12.1.2-0-0
```

After that download this project abd go inside the directory ```Wls-Maven```. Edit the pom as per configuration and execte below mvn cmd.
```
mvn clean install
```

Weblogic-Maven-Plugin pom configuration details and mention inside ```Wls-Maven``` project.
