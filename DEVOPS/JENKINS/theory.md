# Jenkins and Maven

[back](Introduction.md)

## What is Maven?

Maven is commonly referred to as a build tool that is used to manage the entire life cycle of a project, 
generate reports, and store documents with its POM repository.


#### What is POM (Project Object model) file.

Every Maven project directory needs a pom.xml file. These files contain all details necessary for Maven to effectively execute a project. \
The POM file is stored in 'src' or in the root directory

#### Maven build lifecycle

1. Validate : Validate the project is correct and all necessary information is available
2. Compile : During the compile phase, Maven will compile all .java files present in the main directory into .class files and put them back into the main directory in the dedicated folder.
3. Test : During the test phase, Maven will execute the specified test cases and create a summary log.
4. Package : During the package phase, Maven will package all .class files and resources into one file. This file will be formatted into one of the three types given below
    1. ear
    2. war
    3. jar
5. Verify : It runs any checks on results of integration tests to ensure quality criteria are met, at the same time all the previous lifecycle phases are also executed.
6. Install : install the package into the local repository, for use as a dependency in other projects locally, all previous lifecycle phases are also executed.
7. Deploy :It copies the final package to the remote repository for sharing with other developers and projects.


#### Maven repositories

After Maven understands which all dependencies are needed from the pom.xml file, it will download those dependencies from remote repositories and then store them in the local repository for current or future use.


## What is Jenkins

Jenkins is an open-source automation server written in Java. Jenkins helps to automate the nonhuman part of the software development process, with continuous integration and facilitating technical aspects of continuous delivery.


#### Features of Jenkins

Adoption: Jenkins is extremely popular among the open-source community; hence, there are more than 147,000 active installations throughout the world and 1 million people are using it.

Plugins Support: With an extremely active open-source community, Jenkins has around 1000 plugins that allow it to integrate with most of the development, testing and deployment tools.

