cmd has to be in the "real_application" path;
javac -d ../bin com/freimanvs/Main.java
java -cp ../bin com.freimanvs.Main

cmd has to be in the "real_application2" path;
javac -d ../bin com/freimanvs/Main.java com/freimanvs/utils/SomeClass.java
java -cp ../bin com.freimanvs.Main

Create a jar:
cmd has to be in the "real_application2" (or any other) path;
cd ../bin
jar cf myjar.jar com/freimanvs/Main.class com/freimanvs/utils/SomeClass.class

Launch a .jar:
cmd has to be in the path with a .jar file;
java -cp myjar.jar com.freimanvs.Main

several jars...
java -cp jar1.jar;jar2.jar;. com.to.thepackage.Main

