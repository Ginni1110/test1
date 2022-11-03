run the program
javac -cp "src:lib/*" -d out src/ClassmingEntry.java
java -cp "out:lib/*:/Library/Java/JavaVirtualMachines/adoptopenjdk-8.jdk/Contents/Home/jre/lib/rt.jar" ClassmingEntry (MacOS)
java -cp "out:lib/*:/$JAVA_HOME/jre/lib/rt.jar" ClassmingEntry (Linux)

look up JVM versions
/usr/libexec/java_home -V(MacOS)

run:
java -Xbootclasspath/a:/usr/local/java/jdk1.8.0_301/jre/lib/rt.jar -classpath ./sootOutput/avrora-cvs-20091224/:usr/local/java/jdk1.8.0_301/jre/lib/rt.jar  -noverify avrora.Main
java -Xbootclasspath/a:../dependencies/guava-r07.jar:../dependencies/constantine.jar:../dependencies/jnr-posix.jar:../dependencies/jaffl.jar:../dependencies/jline-0.9.95-SNAPSHOT.jar:../dependencies/antlr-3.1.3.jar:../dependencies/asm-3.1.jar:/usr/local/java/jdk1.8.0_301/jre/lib/rt.jar -classpath ../sootOutput/jython/  -noverify org.python.util.jython

/usr/local/java/jdk1.8.0_301/bin/java -Xbootclasspath/a:/usr/local/java/jdk1.8.0_301/jre/lib/rt.jar -classpath ./sootOutput/eclipse/  -noverify org.eclipse.core.runtime.adaptor.EclipseStarter
-Xbootclasspath/a: -classpath "./sootOutput/eclipse/" org.eclipse.core.runtime.adaptor.EclipseStarter -debug