# maven-repository
Self-built maven repository

Notice that snapshots and releases will NOT be distinguished  
For more information, please refer to the details in each second-level headings

**Symbol Interpretations**
- [:scroll: - Project Type]
- [:page_facing_up: - Project URL]
- [:bookmark_tabs: - Usage]
- [:package: - Artifact Information]

**Maven Repo**

```xml
<repository>
	<id>freeze-dolphin's maven repository</id>
	<url>https://raw.github.com/freeze-dolphin/maven-repository/master/repository</url>
</repository>
```
Add this to your `pom.xml` as a dependency  
If you want to create your project from a archetype, you DO NOT need to do this

# containments
## taboolib-quick-start
<details>
    <summary> Details </summary>
    
</details>
[:scroll:] Maven Archetype  
[:page_facing_up:] [github.com/freeze-dolphin/taboolib-quickstart-archetype](https://github.com/freeze-dolphin/taboolib-quickstart-archetype "Project URL")  
[:bookmark_tabs:] Creating from this archetype:  

- You can easily use the "Add Archetype" feature provided by common java ides like Eclipse and IntelliJ to use this archetype
- If you want to generate a project from this archetype in console or terminal: 
  1. Run `mvn org.apache.maven.plugins:maven-archetype-plugin:2.4:generate -DarchetypeGroupId=io.freeze-dolphin.archetypes -DarchetypeArtifactId=taboolib-quickstart-archetype -DarchetypeVersion=1.1.0 -DarchetypeRepository=https://raw.github.com/freeze-dolphin/maven-repository/master/repository/`  
  (Make sure that maven-archetype-plugin v2.x is used while generating, v3.x can not specify the repository url)
  2. Configure the properties for the project
  3. Start coding
</details>

## cyan-core

<details><summary>Details</summary>
[:scroll:] Lib  
[:page_facing_up:] [github.com/freeze-dolphin/CyanCore](https://github.com/freeze-dolphin/CyanCore "Project URL")  
[:bookmark_tabs:] Adding as a dependency: 

```xml
<dependency>
	<groupId>io.freeze-dolphin</groupId>
	<artifactId>cyan-core</artifactId>
	<version>1.0.0</version>
	<scope>`provided`</scope>
</dependency>
```

</details>

