# InnoSetup

generate EXE = mvn jfx:native

#ERROS               |   #Solution
cannot load jvm.dll        |    move your eclipse in ordner programme Files (and not in programme x86); 
						   |	add the following line in eclipse.ini: 
						   |	 	-vm
						   |		C:\pathToJdk\jre\bin\server\jvm.dll  
