# ZenJava generiert eine exe (Not installer => if you click on it it directly start the programm)
    to see how to create an installer take a look in InnoSetup
### configure plugin
    <plugin>
           <groupId>com.zenjava</groupId>
           <artifactId>javafx-maven-plugin</artifactId>
           <version>8.8.3</version>
           <configuration>
               <vendor>our company</vendor>
               <mainClass>foo.bar.MainClass</mainClass>
               <!-- win.app | linux.app | mac.app | exe | msi | rpm | deb -->
               <bundler>win.app</bundler>
           </configuration>
    </plugin>

### Adding icon to .exe
    -> Create src/main/deploy/package/windows/ folder
    -> Add icon with name ${project.build.finalName}.ico
    -> Run mvn jfx:build-native

### Just generate  an exe
    mvn jfx:native
