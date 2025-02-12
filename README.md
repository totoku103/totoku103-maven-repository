# Template
mvn install:install-file -DgroupId= -DartifactId= -Dversion=1.0.0 -Dpackaging=jar -Dfile= -DgeneratePom=true

# Example
mvn install:install-file \
    -DgroupId=me.totoku103 \
    -DartifactId=artifact \
    -Dversion=0.0.1 \
    -Dpackaging=jar \
    -Dfile=artifact-0.0.1.jar \
    -DgeneratePom=true \
    -DlocalRepositoryPath=~/Download

# Reference
http://maven.apache.org/plugins/maven-install-plugin/usage.html


``` xml
pom.xml

<repositories>
    <repository>
        <id>totoku103-repo-snapshot</id>
        <url>https://github.com/totoku103/totoku103-maven-repository/raw/main/releases</url>
    </repository>
</repositories>
```
