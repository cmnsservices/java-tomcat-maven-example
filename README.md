# java-tomcat-maven-example

This is an example ready-to-deploy java web application built for Tomcat using Maven and webapp-runner.
Test Push one
## Running Locally
This is an example ready to deploy java web app built for tomcat 
(need maven and java installed)

```    
mvn packageskdjfnvljksdnvljksdnvkls
mvn package
java -jar target/dependency/webapp-runner.jar target/*.war
```
SampleREADTEST

SampleREADTEST1

SampleREADTEST2

SampleREADTEST3

SampleREADTEST4

SampleREADTEST5
SampleREADTEST5
The application will be available on `http://localhost:8080`.

## How This Was Built in this project test

1. Generate the project using a Maven archetype:

   ```
   test
   mvn archetype:generate -DarchetypeArtifactId=maven-archetype-webapp
  
  viewer

2. Add the webapp-runner plugin into the `pom.xml`:::::

   ```
   <build>
     <!-- ... -->
     <plugins>
       <!-- ... -->
       <plugin>
         <groupId>org.apache.maven.plugins</groupId>
         <artifactId>maven-dependency-plugin</artifactId>
         <version>2.3</version>
         <executions>
           <execution>
             <phase>package</phase>
             <goals><goal>copy</goal></goals>
             <configuration>
               <artifactItems>
                 <artifactItem>
                   <groupId>com.github.jsimone</groupId>
                   <artifactId>webapp-runner</artifactId>
                   <version>8.5.11.3</version>
                   <destFileName>webapp-runner.jar</destFileName>
                 </artifactItem>
               </artifactItems>
             </configuration>
           </execution>
         </executions>
       </plugin>
     </plugins>
   </build>
   ```testing
   
