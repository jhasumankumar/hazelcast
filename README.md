#    Sbring Boot Hazelcast server.

### It uses
    Hazalcast 3.7
    Spring Boot 1.4.0.RELEASE
    Java 8


#### This application starts primary hazelcast member in cluster 
     Members [1] {
	    Member [10.62.25.3]:5701 - 19edcc59-0b45-4115-a0bc-cf2d44dcf896 this
      }

### Configuration - 
    <hz:map name="store">
                <hz:map-store enabled="true" implementation="hazalcastUserCacheStore"
                              write-delay-seconds="0"/> <!--Write-through cache ->

            </hz:map>
            <hz:map name="near">
                <hz:near-cache in-memory-format="OBJECT" max-size="10"/>
            </hz:map> <!--Near cache in object format ->

