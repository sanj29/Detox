> detox

# React Native Demo Project

## Requirements

* Make sure you have Xcode installed (tested with Xcode 8.1-8.2).
* Make sure you have node and npm installed.
* Make sure you have react-native dependencies installed:
   * react-native-cli is installed (`npm install -g react-native-cli`)
   * watchman is installed (`brew install watchman`)

### Step 1: Npm install

* Make sure you're in folder `detox/demo-react-native`.
* Run `npm install`.

## To test Release build of your app
### Step 2: Build 
* Build the demo project
 
 ```sh
 detox build --configuration ios.sim.release
 ```
 
### Step 3: Test 
* Run tests on the demo project``
 
 ```sh
 detox test --configuration ios.sim.release
 ```
 This action will open a new simulator and run the tests on it.

## To test Debug build of your app
### Step 2: Build 
* Build the demo project
 
 ```sh
 detox build --configuration ios.sim.debug
 ```
 
### Step 3: Test 

 * start react-native packager
 
  ```sh
 npm run packager
 ```
 * Run tests on the demo project
 
 ```sh
 detox test --configuration ios.sim.debug
 ```
 This action will open a new simulator and run the tests on it.