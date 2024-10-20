
# compile protobuf definitions
$ pwd
<...>/libsignal-protocol-java

$ tree ./java -L 5 --dirsfirst
./java
├── src
│	├── main
│	│	├── java
│	│	│	└── org
│	│	│		└── whispersystems
│	│	└── main.iml
│	└── test
│		├── java
│		│	└── org
│		│		└── whispersystems
│		└── test.iml
└── ...

## protobuf output directory from the top-level
$ protoc --java_out=./java/src/main/java protobuf/*.proto
