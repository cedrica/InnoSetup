# InnoSetup is use to generate exe installer using UI configuration
      That mean after generate the exe, if the user click on it it will first install the programm on his machine plus a Desktop link to start it.
      But ZenJava donot generate installer but .jar so that if you click on it it directly start the programm

### You can add many things like
      -> icon
      -> licenz ..etc

### ERROS  #Solution cannot load jvm.dll 
-> move your eclipse in ordner programme Files (and not in programme x86); 
-> add the following line in eclipse.ini: 
      -vm  C:\pathToJdk\jre\bin\server\jvm.dll
