# sonatype-oss-kotlin-parent
a parent pom for easy publishing of pure kotlin projects to sonatype-ossrh

### Provides
* jetbrains ```dokka``` plugin configuration to generate javadoc from kotlin
* ```maven-gpg-plugin``` configuration for code signing
* ```maven-source-plugin``` to provide source jars
* easy version upgrade: all versions are properties you can easily overwrite in your project

### What You Need
* use parent
  ```xml
  <parent>
    <groupId>net.thimmwork</groupId>
    <artifactId>sonatype-oss-kotlin-parent</artifactId>
    <version>1.0</version>
  </parent>
  ```
* ```scm``` tag with links to your source code management
* ```developers``` tag
* ```licenses``` tag  (if your code is under another license than Apache Licence, Version 2.0)

### Release your project
To release your project, use either the ```mvn-release-plugin``` or the profile ```sonatype-oss-release```

### Additional Reference
If this is your first project, read any of these tutorials that will guide you through the process to set up everything you need:
* [Sonatype OSSRH Guide](http://central.sonatype.org/pages/ossrh-guide.html)
* [DZone article by Lubos Krnac](https://dzone.com/articles/deploy-maven-central) 
* [Video tutorial by nyholmnik](https://www.youtube.com/watch?v=bxP9IuJbcDQ)
