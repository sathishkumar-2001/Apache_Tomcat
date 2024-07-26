# installation of Tomcat in ubuntu machine 
# update the system

sudo apt update
sudo apt upgrade

# install java greater the java 11

sudo apt install openjdk-11-jdk

# verify java installation

java --version

# Download Apache Tomcat 

download link -> https://tomcat.apache.org/download-10.cgi

# Extract the Downloaded Archive

tar -xvzf apache-tomcat-10.1.26.tar.gz 

# Set Up Environment Variables

echo 'export CATALINA_HOME=/opt/apache-tomcat-10.0.10' >> ~/.bashrc
source ~/.bashrc

# Start Tomcat

cd $CATALINA_HOME/bin
./startup.sh

# Verify Tomcat Installation

Open your web browser and go to http://localhost:8080. You should see the Tomcat welcome page.


