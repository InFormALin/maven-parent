# InFormALin Maven Parent
The Parent for all (sub) projects of InFormALin.

![Maven Deploy (Dev)](https://github.com/InFormALin/maven-parent/workflows/Maven%20Deploy%20(Dev)/badge.svg)

## HowTo
1. Always use `edu.kit.kastel.[subproject]` as group id and an arbitrary artifact id that defines your project
2. Then just add the dependency to this parent (you may use your own parent that inherits from this parent):

```xml
<repositories>
	<repository>
		<id>github</id>
		<name>GitHub InFormALin-Parent Apache Maven Packages</name>
		<url>https://maven.pkg.github.com/InFormALin/maven-parent</url>
	</repository>
</repositories>

<parent>
	<groupId>edu.kit.kastel.informalin</groupId>
	<artifactId>parent</artifactId>
	<!-- Just use the version you want. -->
	<version>0.3-SNAPSHOT</version>
</parent>
```
