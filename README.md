Q2: Adding Apache Commons Lang Dependency and Repository

The Apache Commons Lang dependency and its corresponding repository URL have been included in the parent module's pom.xml file.

Dependency Added: Apache Commons Lang (Version 3.12.0)

Repository URL: https://commons.apache.org/proper/commons-lang/

Location: pom.xml (parent module)

Q3: Adding JitPack Repository and Using Its Dependency

The JitPack repository has been integrated into the parent module's pom.xml file. A dependency from GitHub, named JitPackDemo, has also been added.

Repository Added: JitPack Repository

Dependency Used: JitPackDemo (Version 1.0)

Location: pom.xml (parent module)

Q4: Configuring Maven JAR Plugin to Create an Executable JAR

In the pom.xml file of the SubClass1 module, the Maven JAR Plugin has been configured to produce an executable JAR. This configuration specifies the main class to be executed.

Maven Plugin Used: Maven JAR Plugin (Version 3.2.0)

Main Class Defined: com.ttn.SubClass1.App

Execution Command: java -jar SubClass1/target/SubClass1-1.0-SNAPSHOT.jar

Expected Output: "Hello from SubClass1"

Location: pom.xml (SubClass1 module)

Q5: Explanation of Different Dependency Scopes

Various dependency scopes are defined in the parent module's pom.xml file:

Compile Scope: Dependencies required during both compilation and runtime.

Example: SLF4J (Simple Logging Facade for Java)

Runtime Scope: Dependencies needed only during runtime, not at compile-time.

Example: MySQL Connector (for database connections)

Test Scope: Dependencies used exclusively for testing purposes.

Example: JUnit (for unit testing)

Provided Scope: Dependencies provided by the runtime environment and not included in the final package.

Example: Servlet API (for web applications)

Location: pom.xml (parent module)

Q6: Creating a Multi-Module Project and Packaging All Modules

A multi-module Maven project has been created, which consists of two child modules: SubClass1 and SubClass2. Upon packaging, JAR files are generated for each module.

Modules Created: SubClass1, SubClass2

Execution Command: mvn clean package

Expected Outcome:

JAR files for both modules.

Output JARs are stored in the target folders of the respective child modules.

(Note: The target folder is excluded from the Git repository as per the provided instructions.)

Location: target folders (within SubClass1 and SubClass2 modules)

Referenced URLs:

Maven Official Documentation: http://maven.apache.org

JitPack: https://jitpack.io

Apache Commons Lang: https://commons.apache.org/proper/commons-lang/

SLF4J: http://www.slf4j.org/

JUnit: https://junit.org/junit4/

MySQL Connector: https://dev.mysql.com/downloads/connector/j/

Java EE Specification: https://javaee.github.io/javaee-spec/
