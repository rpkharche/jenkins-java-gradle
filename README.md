# jenkins-java-gradle
This is a jenkins project with gradle as build system

# Enable Java Plugins 
```
apply plugin: 'java'
```

# Maven repositories 
```
repositories {
   jcenter()
}
```
# Maven dependancies
```
dependencies {
   compile 'org.slf4j:slf4j-api:1.7.12'
   testCompile 'junit:junit:4.12'
}
```
# Gradle Tasks Demo - Hello World
```
task hello {
	doLast{
		println 'Hello World'
	}
}
```
# Gradle Tasks Demo - Groovy 
```
task upper << {
	String expString = 'Ravindra'
	println 'Original:' + expString
	println 'Upper Case:' + expString.toUpperCase()
}
```
# Gradle Tasks Demo - Groovy Iterations
```
task count << {
	4.times{
		print "$it"
	}
}
```
# Gradle Tasks Demo - GroovyJDK
```
task tokenizeName << {
	String name = "Ravindra"
	name.each(){
		println "$it"
	}
}
```
