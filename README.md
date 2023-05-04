# Ubuntu Environment Setup For Flutter


Before Running Any Command You Need To Run

```
 sudo apt update
```

# Curl

### Install

```
sudo apt install curl
```

# Flutter

## Install Flutter manually

- [Visit](https://docs.flutter.dev/get-started/install/linux) & Download the installation bundle to get the latest stable release of the Flutter SDK

- After Download the SDK Create Folder For Flutter Environment.
- Move & Extract The Downloaded File in the new created folder
- Go to the bin folder in flutter and copy the path directory and paste that in `.bashrc` file.

```
export PATH="$PATH:`path/bin"
```
 
- Type `flutter` in the trminal and run for check the flutter installation

 - Pre-download development binaries:
```
flutter precache
```
- Run the following command to see if there are any dependencies you need to install to complete the setup

```
flutter doctor
```

## Install Android Studio
### Install JDK

```
sudo apt install openjdk-11-jdk
```

### Add android-studio repository

```
sudo add-apt-repository ppa:maarten-fonville/android-studio
```

```
sudo apt update
```

### Install Android Studio

```
sudo apt install android-studio -y
```

In Android Studio
- Install Android SDK Command-line Tools (Latest)
- Install Flutter Plugin

### Agree to Android Licenses
```
flutter doctor --android-licenses
```

### Additional Linux requirements
```
sudo apt-get install clang cmake ninja-build pkg-config libgtk-3-dev liblzma-dev
```