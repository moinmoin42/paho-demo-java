- edit the code, create a class with a `main` in it -> `MqttPublishSample.java`
- write a manifest file, name it `META-INF/MANIFEST.MF` and its contents must end with a `\n`
- the contents of the manifest file
```
Main-Class: MqttPublishSample
Class-Path: org.eclipse.paho.client.mqttv3-1.2.1.jar
```
- `javac MqttPublishSample.java` -> this produces `MqttPublishSample.class` in the same directory
- `jar cmvf META-INF/MANIFEST.MF out.jar org.eclipse.paho.client.mqttv3-1.2.1.jar MqttPublishSample.class`  -> this will build one Jar with everything in it
- run `java -jar out.jar` to execute the resulting file

