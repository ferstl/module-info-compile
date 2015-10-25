# module-info-compile
*- Use maven to compile `module-info.java` with source level 1.9 while compiling the rest of the code with lower source levels*


### How does it work
The compilation is split into two steps. The first step compiles the source files with the configured source level.
The second stap compiles the `module-info.java` with source level 1.9 . Additionally, maven's *default-compile* execution
has to be disabled.

Take a look at the [POM](pom.xml) file to see the details.
