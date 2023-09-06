# What is Maven?
Apache Maven is a popular build tool, that takes your project's Java source code, compiles it, tests it and converts it into an executable Java program, which is either a `.jar` or `.war` file.

`mvn clean install` is the command to just to that.
1. You are calling the `mvn` executable.
2. You are using the `clean` command, which delete previously compiled Java `.class` files and resources like `.properties` in your project. 
3. `install` will compile, test & package your Java project and even install/copy your built `.jar` or `.war` file into your local Maven repository. 
~
# How to initialize an empty folder as a Maven project?


1. Open your command line or terminal and navigate to the root folder of your dedicated project folder.
2. Run the following command to initialize the project:
	
	```shell
D:\practice\java\fun\mp3-project>mvn archetype:generate -DgroupId=com.mp3ditor -DartifactId=mp3ditor -DarchetypeArtifactId=maven-archetype-quickstart -DinteractiveMode=false -Dmaven.plugin.validation=VERBOSE
```

	*This command uses the Maven archetype `maven-archetype-quickstart` to generate a basic project structure. Feel free to modify the `groupId` and `artifactId` parameters according to your project's information.*

	<blockquote style="color: #999;"> 
		<i>
			📖❓ What's that  <code>interactiveMode=false</code>?<br>
			<p>The `interactiveMode=false` flag is used in Maven commands to specify non-interactive mode. By default, Maven runs in interactive mode, which means it prompts you for input when generating a project from an archetype.
			</p>
			<p>
			When you set <code>interactiveMode=false</code>, it instructs Maven to run in non-interactive mode, bypassing any prompts and using default values for project generation.
			</p>
			<p>
			❗ However, keep in mind that using <code>interactiveMode=true</code> means that you accept default values provided by the archetype, which may or may not suit your specific project requirements
			</p>
		</i>
	</blockquote>


3. Maven will create the project structure and add the files for you. You should see a new folder named after your `artifactId` (`mp3ditor` in this example) in your dedicated folder.

4. The project's main Java file can be found at `src/main/java/com/mp3ditor/App.java`. You can modify this file or create additional Java files in the appropriate directories 

# What does the `pom.xml` do?
~

# What is a Maven wrapper `mvnw` ?  

# Maven Commands
~
`mvn wrapper: wrapper`
`mvn validate`
`mvn compile`
`mvn test`
`mvn compile test`


