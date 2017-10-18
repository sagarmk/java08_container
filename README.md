# java08 container
---
### To build image:
```
git clone https://github.com/sagarmk/java08_container.git 

docker build -f Dockerfile -t sagarmk/java08_container:8 . 
```

### To compile java file:

```
docker run --rm -v $PWD:/app -w /app sagarmk/java08_container:8 javac Main.java 
```

### To run a compiled java file:
```
docker run --rm -v $PWD:/app -w /app sagarmk/java08_container:8 java Main
```
