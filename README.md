<p align="center">
  <img width="200" height="200" src="https://github.com/usmankhi18/CalculatorApp/blob/master/resources/icon.png">
</p>

Installation:

    ionic plugin add https://github.com/usmankhi18/MathCalculator.git


Supported Platforms:

    Android


Plugin usage:

          add()
          {
              let data = {
                  param1: this.param1,
                  param2: this.param2
               }
              this.math.add(data).then(result => {
              this.answer = result;
              }).catch(err => alert("Error : " + err));
          }
          
          substract()
          {
              let data = {
                param1: this.param1,
                param2: this.param2
              }
              this.math.substract(data).then(result => {
              this.answer = result;
              }).catch(err => alert("Error : " + err));
          }

          multiply()
          {
              let data = {
                param1: this.param1,
                param2: this.param2
              }
              this.math.multiply(data).then(result => {
              this.answer = result;
              }).catch(err => alert("Error : " + err));
          }
  
          divide()
          {
              let data = {
                  param1: this.param1,
                  param2: this.param2
              }
              this.math.divide(data).then(result => {
              this.answer = result;
              }).catch(err => alert("Error : " + err));
          }
            
Create Plugin Process: 

    1. Install Node JS
        https://nodejs.org/en/


    2. npm install -g plugman

    3. Create Plugin
        plugman create --name <pluginName> --plugin_id <pluginID> --plugin_version <version> [--path <directory>] [--variable NAME=VALUE]
        plugman create --name Calculator --plugin_id cordova-plugin-calculator --plugin_version 1.0.0

    4. Go Inside Directory / add platforms

    5. In plugin.xml , correct the path for "target-dir"

    7. In plugin.xml,  correct the  android-package by replacing "-" with "."

    6. in Calculator.java in src. correct the package name by replacing "-" with "."

    7. in Calculator.js, add different methods you wants your plugin to perform.

    8. add defination of all these methods in "Calculator.java" for android and in "Calculator.m" for ios. 

    9. make "clobbers" as as single string like "Calculator" or it will not work.
