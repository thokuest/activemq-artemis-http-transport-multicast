# activemq-artemis-http-transport-multicast

Tweaked `http-transport` example from the ActiveMQ Artemis project that produces and consumes multiple messages from a multicast address/JMS topic via HTTP transport.

Run the example via

```
$ mvn verify
```

ActiveMQ Artemis is downloaded automatically via [download-maven-plugin](https://github.com/maven-download-plugin/maven-download-plugin) and extracted to the project's build directory.
Downloading and extracting can be skipped by property `download.plugin.skip`:

```
$ mvn verify -Ddownload.plugin.skip
```

Optionally, `MessageConsumer.receive()` calls can be delayed (milliseconds):

```
$ mvn verify -DconsumerDelay=1000
```