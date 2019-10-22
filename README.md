# Adding Maven to the Environment Path
```
export M2_HOME=/usr/local/apache-maven/apache-maven-3.3.9
export M2=$M2_HOME/bin
export PATH=$M2:$PATH 
mvn -version
```

# Generate maven project template
```
mvn archetype:generate
```

#Use different profiles
```
mvn clean package -P prod
mvn clean package -Denv=prod

#Run app
java -jar target/firstTuturial-1.0-SNAPSHOT.jar
```
