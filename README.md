# Shacl Validator

Using this tool you can easily run shacl validations and get reports.

Input shacl and data files can be any type of RDF; output reports are turtle files.

## Using the tool 

From the commandline output

```
usage: java -jar shacl.jar
                [--shacl folder, file or ant-style file pattern] 
                [--validate folder, file or ant-style file pattern ("./conceptscheme/**/*.ttl")] 
optional:       [--destination folder] 
```

Example                     

```
java -jar shacl.jar 
   --shacl ./shacl-examples/*.ttl 
   --validate ./skos/*.ttl
```

will start and show

```
Running with settings: 

		 Shacl           : ./shacl-examples/*.ttl
		 Validate        : ./skos/*.ttl
		 Destination     : .
```
                      
## Building

A build will create a `shacl.jar` file. 

### On Windows
                      
```
gradlew.bat build
```

### On Unix

```
./gradlew build
```
