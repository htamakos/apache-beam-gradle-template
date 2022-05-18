# ApacheBeam Project Generator
## How to add sub projects

```
$ ./gradlew addSubProject -PappName="App" -PprojectName="sample1"
```

create projects like below.

```
./sample1
├── build.gradle
└── src
    ├── main
    │   ├── java
    │   │   └── dataflow
    │   │       └── java
    │   │           └── samples
    │   │               └── App.java
    │   └── resources
    └── test
        ├── java
        │   └── dataflow
        │       └── java
        │           └── samples
        │               └── AppTest.java
        └── resources
```

And append subproject line like below.

```
...
include('sample1')
```
