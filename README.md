# spring-vue-template
Empty Template for quick setup of a Spring Boot Vuejs Application

To get your project up and running you only have to edit the following files:

## root/pom.xml
  * Update the Maven details
    * groupId
    * artifactId
    * version
    * name
    * description
    
## backend/pom.xml
  * Update the `<parent> ` tags to match root
    * groupdId
    * artifactId
    * version
    
  * This pom file includes javassist which is required if you are using JDK11
  
## frontend/pom.xml
  * Update the `<parent> ` tags to match root
    * groupdId
    * artifactId
    * version
  * nodeVersion to match your desired version
  
## frontend/package.json
  * Name
  * Description
  * Author
  
## backend/src
  * package "project_name"
  * MainApplication.java to something more relevant to you application.
  * resources/application.properties
    * **This uses postgres for a database because that's what comes with Heroku out of the box. You will need to create the database and userusername in pgAdmin before this will work**
    * DB_NAME: spring.datasource.url=jdbc:postgresql://localhost:5432/DB_NAME
    * USERNAME: spring.datasource.username=USERNAME
    * PASSWORD: spring.datasource.password=PASSWORD
  
# Running Backend
**Note**: I'm using IntelliJ community.

Open project > Select the pom.xml in the root directory > Open as Project.

Right click backend/src/main/java/com/jcromp.project_name.MainApplication.java > Run

# Running Frontend

In the terminal cd into frontend
` npm run dev` 

And you are up and running.

