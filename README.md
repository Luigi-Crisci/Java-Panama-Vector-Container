# Panama Vector container
A simple container with OpenJDK Panama Vector installed.

## How to build and run the container

### Build
A pre-built image can be found in docker hub. You can obtain it by typing:
```bash
docker pull luigicrisci/panama-vector
```
or you can build it on your own with:
```
git clone https://github.com/Luigi-Crisci/Java-Panama-Vector-Container/
cd Java-Panama-Vector-Container
docker build -t YOUR_IMAGE_NAME .
```

### Run
Run the image and create a container by typing:
```
docker run -it YOUR_IMAGE_NAME
```


## How to build the examples
From within the container, type:
```bash
git clone https://github.com/Luigi-Crisci/Java-Panama-Vector-Container/
cd Java-Panama-Vector-Container
javac --add-modules=jdk.incubator.vector examples/VectorTest.java -d examples/
```
and run it with:
```bash
java --add-modules=jdk.incubator.vector -cp examples VectorTest
```

## Useful materials on the Panama Vector Project
- [Vector API: Writing own-vector algorithms in OpenJDK for faster performance](https://www.intel.com/content/dam/develop/public/us/en/documents/vector-api-writing-own-vector-final-9-27-17.pdf) (2017, quite old)
- [Vector API Developer Program for Java* Software](https://www.intel.com/content/www/us/en/developer/articles/technical/vector-api-developer-program-for-java.html)
- [Panama vector benchmark](https://github.com/JOML-CI/panama-vector-bench)
- [Java Vector API: Intel talk](https://www.youtube.com/watch?v=YA9wfTrBr_4)
- [Java Vector API: Oracle talk](https://www.youtube.com/watch?v=1JeoNr6-pZw)
