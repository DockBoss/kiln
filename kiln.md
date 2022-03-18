# Running Nethermind on Kiln
## Windows
### setting up secret TODO:
write how to download openssl and how to create random hex file
### Downloading and Building Nethermind from Source
Clone Nethermind from github
```
git clone -b kiln https://github.com/NethermindEth/nethermind.git --recursive
```
requirements to build
* .NET SDK 5.0
* Maybe also VS not sure what year
make you are in the right directory before you start building
```
cd nethermind/src/Nethermind
dotnet build Nethermind.sln -c Release
```
Start client
```
cd Nethermind.Runner
dotnet run -c Release --no-build --config kiln --JsonRpc.JwtSecretFile=C:\Users\jared\dev\Kiln\jwtSecret
```
### Downloading Lighthouse

### Downloading Lodestar
### Downloading Prysm
### Downloading Teku
#### Prerequisites
* [Java JDK](https://www.oracle.com/java/technologies/downloads/)
  * Java 11+ supported
* [Git](https://git-scm.com/downloads)
* [Gradle](https://gradle.org/)
#### Building Teku
```
git clone https://github.com/Consensys/teku.git
cd teku
./gradlew distTar installDist
cd build/install/teku
bin/teku --help
```

### Downloading Nimbus
## Linux
### Downloading Nethermind from Source
### Downloading Lighthouse
### Downloading Lodestar
### Downloading Prysm
### Downloading Teku
### Downloading Nimbus