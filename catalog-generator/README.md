# WildFly catalog generator

## Build the project

`mvn clean install`

## Generate a local catalog

NOTE: Local testable catalog implies that your web browser has access to the file system from javascript. For example, launch `chrome` with the option 
`--allow-file-access-from-files`

* `mvn exec:java -Dwildfly-version=<WildFly Version>`

* You can then access the catalog by browsing the local file `target/catalog/<wildfly version>/index.html`

## Generate the catalog to be deployed

`mvn exec:java -Dwildfly-version=<WildFly Version> -Drelease=true`

The directory `../docs/` is updated with the generated catalog`
