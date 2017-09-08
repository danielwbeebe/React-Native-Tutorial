# REACT NATIVE TUTORIAL

By Militsa Neykova & Dan Beebe

## Introduction

React Native is a framework used to construct mobile applications written in JavaScript, utilizing the React library to create the user interface. 

According to Facebook's documentation on React Native:

"With React Native, you don't build a 'mobile web app', an 'HTML5 app', or a 'hybrid app'. You build a real mobile app that's indistinguishable from an app built using Objective-C or Java. React Native uses the same fundamental UI building blocks as regular iOS and Android apps. You just put those building blocks together using JavaScript and React."

In other words, although React Native apps are written in JavaScript, their structure is essentially the same as other apps.

This tutorial includes sections on: (i) why you might want to use React Native; (ii) getting started with React Native; (iii) specific code examples; and (iv) resources for further reading.

## Why Use React Native?

Although the React apps are fundamentally made from the same building blocks as a native app, they are (arguably) better and faster. React Native applications can be much easier to code, less expensive, and save you a lot of time. It's all open source. One of the most valiable features that React gives to programmers is that it makes the views layers output of the states.
   
## Getting Started

To start using React Native, you should install the React Native npm package by running the following code in your terminal:

        npm install -g react-native-cli

You'll also want to install yarn to help with setting up your React Native App, so run the following too:

        npm install -g yarn

To initialize a new React Native app, go into the folder where you want to create your app and run the following command:

        react-native init newAppName

To work on your app, you should also make sure you have Java downloaded and set up an android virtual device on your computer. (See resources section below.)

## Code Examples 

// The examples are taken from the tutorial https://www.youtube.com/watch?v=mkualZPRZCs&t=1704s

Here are a few examples of code in React Native: 

First, this code must be added to render the app using React Native in the index file:

        import {AppRegistry, Text, View} from 'react-native'

Rendering the information (also in the index file):

        export default class newAppName extends Component {
           render(){
              return(
                 <View>
                   <Text>Hello World!</Text>
                 </View>
              );
           }
        }

Registering the application (also in the index file):

        AppRegistry.registerComponent('newAppName', () => myapp);


The Programmer can use props and state (just like in React):

         export default class newAppName extends Component {
           constructor(){
             super();
             this.state = {
                name: 'Michael'
             }
            }

           render(){
             return(
               <View>
                 <Text>{this.props.message}</Text>
                 <Text>{this.state.name}</Text>
                 </View>        
              );
            }
          }

## Resources

### To Read
[React Native Official Site](http://www.reactnative.com/)

[Facebook's Tutorial on React Native](https://facebook.github.io/react-native/docs/tutorial.html)

### To Watch
[React Native Crash Course YouTube Video](https://www.youtube.com/watch?v=mkualZPRZCs)

[Video on Android SDK & AVD Setup For React Native](https://www.youtube.com/watch?v=KRLLjlpy0r4)

### To Download
[NPM Page for React-Native-Cli Package](https://www.npmjs.com/package/react-native-cli)

[Download Java](http://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.htm)

[Download Android Studio](https://developer.android.com/studio/install.html)
