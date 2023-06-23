**Maven Install Step**
- sudo su
- cd /opt
- ll
- wget https://dlcdn.apache.org/maven/maven-3/3.9.2/binaries/apache-maven-3.9.2-bin.tar.gz
- tar -xvzf apache-maven-3.9.2-bin.tar.gz
- mv apache-maven-3.9.2 maven
- cd maven
- cd bin
- ./mvn -v

**Setup Env Variables**
- cd ~
- pwd
- ll -a
- vi .bash_profile
  - Inside the above file set below env
  - M2_HOME=/opt/maven
  - M2=/opt/maven/bin
  - (Find the Java Install path using find/ -name jvm)
    - cd /usr/lib/jvm
    - find / -name java-11*
  - Setup below env for Java
  - JAVA_HOME=/usr/lib/jvm/java-11-openjdk-11.0.19.0.7-1.amzn2.0.1.x86_64
  - PATH=$PATH:$HOME/bin:$JAVA_HOME:$M2_HOME:$M2
  - Save the .bash_profile
  - source .bash_profile
  - Check env set properly
  - echo $PATH
 
  **Install Maven Integration**
  
    
