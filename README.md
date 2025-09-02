# unmeshed-java-sdk

### Instructions to build

Create a Public Private key using Gpg and define sig3 Short using below short command in pom

Use some config in pom

See below helpful config and commands for reference

```
gpg --list-keys
gpg --list-signatures --keyid-format 0xshort
gpg --keyserver keyserver.ubuntu.com --send-keys ...


mvn clean
mvn package


export AWS_ACCESS_KEY_ID=<accessKey>
export AWS_SECRET_ACCESS_KEY=<secretKey>
export AWS_REGION=<awsRegion>

export GPG_KEYNAME=<gpgSig3KeyName>
export GPG_PASSPHRASE=<gpgPassPhrase>

export REVISION=<semantic revision like x.y.z>



mvn deploy
```