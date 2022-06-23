# Panama Vector container
A simple container with OpenJDK Panama Vector installed.

## How to build the examples
From the root folder, type:
```bash
javac --add-modules=jdk.incubator.vector examples/VectorTest.java -d examples/
```
and run it with:
```bash
java --add-modules=jdk.incubator.vector -cp examples VectorTest
```
