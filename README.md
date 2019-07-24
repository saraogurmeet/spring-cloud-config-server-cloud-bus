# spring-cloud-config-server
This is a sample project that uses the Spring Cloud Config to create a config server. I have used the Spring Security to secure the communication between clients and server. In addition to this, I am using Github as the config repository where both plain and encrypted properties are stored. We are using asymmetric encryption for more security. Please find below the command to create the jks that can be found in src/main/resources.
use the following command to generate jks if and when needed:
keytool -genkeypair -alias config-server-key -keyalg RSA -keysize 4096 -sigalg SHA512withRSA -dname 'CN=Config Server,OU=Spring Cloud,O=Baeldung' -keypass my-k34-s3cr3t -keystore config-server.jks -storepass my-s70r3-s3cr3t

This project references and uses parts of Baeldung at link: https://www.baeldung.com/spring-cloud-configuration
