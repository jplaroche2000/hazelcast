FROM hazelcast/hazelcast:3.12.2

# Adding custom hazelcast.xml
ADD hazelcast.xml ${HZ_HOME}
ADD config ${HZ_HOME}/config
ADD user-lib ${HZ_HOME}/user-lib

ENV CLASSPATH ${CLASSPATH}:${HZ_HOME}/config:${HZ_HOME}/user-lib/*

ENV JAVA_OPTS -Dhazelcast.config=${HZ_HOME}/hazelcast.xml

