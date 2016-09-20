FROM java:latest

COPY src/HelloWorld.java /home/root/javahello/src/
#COPY src /home/root/javahello/src

WORKDIR /home/root/javahello
COPY bin /home/root/javahello/bin
RUN javac -d bin src/HelloWorld.java

COPY src /home/root/javahello/src

ENTRYPOINT ["java", "-cp", "bin", "HelloWorld"]
