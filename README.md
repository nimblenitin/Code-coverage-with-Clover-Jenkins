# Code-coverage-with-Clover-Jenkins

Clover is a tool that generates Test Coverage reports. Steps to perform code coverage using Clover in Jenkins for a Maven application 

```

1. Create a new Maven project in Eclipse IDE.

2. Add the xml from this Github repo to the .pom file in the project created. Save and update the Maven project.

3. In Jenkins under manage plugin add Clover plugin

4. Create a Maven item, in build section add the path of the .pom file and specify the below goal-
install -Dmaven.test.failure.ignore=true clover:instrument clover:aggregate -N clover:aggregate clover:clover

5. Run the job and view the console output.

```


