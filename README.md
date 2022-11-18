# scratch docker example

## Compile

`g++ -o hello hello.cpp`

MacOS can not static link gcc lib

though docker gcc compile the source code

`docker run --rm -v "$PWD":/usr/src/myapp -w /usr/src/myapp gcc g++ -o hello -static hello.cpp`

## Build and Run

`docker build --tag hello-scratch-docker .`

`docker run hello-scratch-docker`
