# maven-repository
This is my self-built maven repository

Notice that `snapshots` and `releases` **will NOT** be distinguished and all updates will be published in the branch `master`

For more information, please refer to the details in each second-level headings

**Symbol Interpretations**

- [:scroll: - `Project Type`]
- [:page_facing_up: - `Project URL`]
- [:bookmark_tabs: - `Usage`]
- [:package: - `Artifact Information`]
- [:warning: - `Attentions & Warnings`]

**Maven Repository**

```xml
<repository>
	<id>freeze-dolphin's maven repository</id>
	<url>https://raw.github.com/freeze-dolphin/maven-repository/master/repository/</url>
</repository>
```
Add this to your `pom.xml` as a dependency

If you want to create your project from a archetype, you **DO NOT** need to do this

## attentions

As if you cannot have access to `raw.github.com` conveniently, you can use the following one instead: 

```xml
<repository>
	<id>freeze-dolphin's maven repository</id>
	<url>https://raw.sevencdn.com/freeze-dolphin/maven-repository/master/repository/</url>
</repository>
```

# containments
## taboolib-quick-start
<details>
    <summary> Details </summary>

[:scroll:] Maven Archetype

[:page_facing_up:] [github.com/freeze-dolphin/taboolib-quickstart-archetype](https://github.com/freeze-dolphin/taboolib-quickstart-archetype "Project URL")

[:bookmark_tabs:] Creating from this archetype: 

- You can easily use the "Add Archetype" feature provided by common java ides like Eclipse and IntelliJ to use this archetype
- If you want to generate a project from this archetype in console or terminal: 
  1. Run `mvn org.apache.maven.plugins:maven-archetype-plugin:2.4:generate -DarchetypeGroupId=io.freeze-dolphin.archetypes -DarchetypeArtifactId=taboolib-quickstart-archetype -DarchetypeVersion=1.1.0 -DarchetypeRepository=https://raw.github.com/freeze-dolphin/maven-repository/master/repository/`  
  (Make sure that `maven-archetype-plugin` **v2.x** is used while generating, v3.x **can not** specify the repository URL)
  2. Configure the properties for the project
  3. Start coding

[:warning:] If you have problems in getting access to `raw.github.com`, please change the `archetypeRepository` to `https://raw.sevencdn.com/freeze-dolphin/maven-repository/master/repository/`  which is mentioned above

</details>

## cyan-core

<details>
    <summary>Details</summary>

[:scroll:] Lib

[:page_facing_up:] [github.com/freeze-dolphin/CyanCore](https://github.com/freeze-dolphin/CyanCore "Project URL")

[:bookmark_tabs:] Adding as a dependency: 

```xml
<dependency>
	<groupId>io.freeze-dolphin</groupId>
	<artifactId>cyan-core</artifactId>
	<version><!-- VERSION HERE --></version>
	<scope>provided</scope>
</dependency>
```

</details>

