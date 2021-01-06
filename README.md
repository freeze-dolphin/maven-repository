# maven-repository
Self-built maven repository

Notice that snapshots and releases will NOT be distinguished  
For more information, please refer to the details in each second-level headings

**Symbol interpretations**
- [:scroll: - Project Type]  
- [:page_facing_up: - Project URL]  
- [:package: - Usage]

**Maven Repo**
```xml
<repository>
	<id>freeze-dolphin's maven repository</id>
	<url>https://raw.github.com/freeze-dolphin/maven-repository/master/repository</url>
</repository>
```
Add this to your "pom.xml" as a dependency  
If you want to create your project from a archetype, you DO NOT need to do this

# containments
## taboolib-quick-start
[:scroll:] Maven Archetype  
[:page_facing_up:] [github.com/freeze-dolphin/taboolib-quickstart-archetype](https://github.com/freeze-dolphin/taboolib-quickstart-archetype "Project URL")  
[:package:] Creating from this archetype:  
- You can easily use the "Add Archetype" feature provided by common java ides like Eclipse and IntelliJ to use this archetype
- If you want to generate a project from this archetype in console or terminal: 
  1. Run `mvn org.apache.maven.plugins:maven-archetype-plugin:2.4:generate -DarchetypeGroupId=io.freeze-dolphin.archetypes -DarchetypeArtifactId=taboolib-quickstart-archetype -DarchetypeVersion=1.1.0 -DarchetypeRepository=https://raw.github.com/freeze-dolphin/maven-repository/master/repository/` (Make sure that maven-archetype-plugin v2.x is using while generating, only 2.x can specify the repository url)
  2. Configure the properties for the project
  3. Start coding
