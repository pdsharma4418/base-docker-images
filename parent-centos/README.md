Build java docker image

Download tar.gz from orcale, Save the filename as a variable
export java_filename='jdk-11.0.2_linux-x64_bin.tar.gz'
docker build --build-arg JAVA_PKG="${java_filename}" -t com/company-project-centos-java .

Build tomcat docker image based on com/company-project-centos-java
from tomcat base dir folder 
docker build -t com/company-project-centos-java-tomcat .