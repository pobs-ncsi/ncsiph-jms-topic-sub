# ncsiph-jms-topic-sub

Ref: http://middlewaremagic.com/weblogic/?p=2431

JMS Topic Subcriber Sample Application

$ mvn org.apache.maven.plugins:maven-install-plugin:2.5.2:install-file  -DcreateChecksum=true -DgeneratePom=true -Dpackaging=jar -Dfile=lib/wlclient.jar -DgroupId=weblogic -DartifactId=wlclient -Dversion=10.3

$ mvn org.apache.maven.plugins:maven-install-plugin:2.5.2:install-file  -DcreateChecksum=true -DgeneratePom=true -Dpackaging=jar -Dfile=lib/wljmsclient.jar -DgroupId=weblogic -DartifactId=wljmsclient -Dversion=10.3

$ mvn clean package

$ mvn -Ptopic-subscriber exec:java -Dexec.args=t3://localhost:7001
