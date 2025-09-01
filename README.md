# unmeshed-java-sdk

### Instructions to build

Create a Public Private key using Gpg and define sig3 Short using below short command in pom

Use some config in pom
```
gpg --list-keys
gpg --list-signatures --keyid-format 0xshort
gpg --keyserver keyserver.ubuntu.com --send-keys ...
mvn clean package
mvn deploy
```