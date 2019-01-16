FROM azul/zulu-openjdk:11

COPY /maven/${project.build.finalName}.jar /opt/

USER 1000:1000
EXPOSE 8080
WORKDIR /opt/

ENV TZ=Asia/Shanghai

ENTRYPOINT ["java", "-jar", "${project.build.finalName}.jar"]
