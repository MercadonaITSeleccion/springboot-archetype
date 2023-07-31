FROM docker.artifactory.gcp.mercadona.com/custom/springboot-java:17-jre-alpine-v2

ARG DEPENDENCY=target/dependency

# Add layers which may be cached
COPY ${DEPENDENCY}/org ./org
COPY ${DEPENDENCY}/BOOT-INF/lib ./BOOT-INF/lib

# Add new layers
COPY ${DEPENDENCY}/META-INF ./META-INF
COPY ${DEPENDENCY}/BOOT-INF/classes ./BOOT-INF/classes
