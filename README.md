# awesome-flume-plugins
A curated list of awesome Apache Flume Plugins: sources, sinks, interceptors, serializer, monitoring tools

## Sources


## Sinks

*   [flume-ng-kafka-sink for kafka 0.8.2, 0.9.x, 0.10.x](https://github.com/apache/flume/tree/trunk/flume-ng-sinks/flume-ng-kafka-sink)

Since the builtin flume-ng-kafka-sink in Flume 1.6.0 only support kafka 0.8.1, this if for those whose Kafka cluster >= 0.8.2. If you want to build this plugin with dependencies. replace the `build section` in pom.xml with the following code:

```
<build>  
    <plugins>  
  
        <plugin>  
            <groupId>org.apache.maven.plugins</groupId>  
            <artifactId>maven-assembly-plugin</artifactId>  
            <version>2.5.5</version>  
            <configuration>  
                <descriptorRefs>  
                    <descriptorRef>jar-with-dependencies</descriptorRef>  
                </descriptorRefs>  
            </configuration>  
        </plugin>  
  
    </plugins>  
</build>
```


## Interceptors

*   [Flume Interceptor: Enriched Event](https://github.com/keedio/flume-enrichment-interceptor-skeleton)

*   [flume event header fields copy interceptor](https://github.com/keedio/flume-event-header-fields-copy-interceptor)


## Serializer

*   [HeaderAndBodyTextEventSerializer, JSONEventSerializer](https://github.com/wdavidw/flume)


## Monitoring Tools

*   [Monitoring flume - A event counter](https://github.com/BenJoyenConseil/monitor-flume)
