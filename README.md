# Knowledge Center Javascript Style Guide

## Table of Contents

  1. [Objects](#objects)
  2. [Arrays](#arrays)
  3. [Strings](#strings)
  4. [Functions](#functions)

## Objects

  - [1.1](#1.1) Use the literal syntax for object creation

    ```javascript
    // good
    var batman = {};
    ```
  
  - [1.2](#1.2) Use dot-notation when accessing properties directly
  
    ```javascript
    var id = batman.secretIdentity;
    ```
  - [1.3](#1.3) Use square-bracket notation when access properties with a variable
  
    ```javascript
    var id = batman[secretIdentity];
    ```

## Arrays

  - [2.1](#2.1) Use the literal syntax for array creation
  
  ```javascript
  var utilityBelt = [];
  ```
  
  - [2.2](#2.2) Store the length first to improve performance when iterating through arrays
  
  ```javascript
  var utilityBelt = [];
  var utilityCount = arr.length;
  for(var i = 0; i < utilityCount; i++) {
    \\ ...
  }
  ```

## Strings

  - [3.1](#3.1) Use single quotes `''` for strings.
  
  ```javascript
  batman.secretIdentity = 'Bruce Wayne';
  ```
## Functions

  - [4.1](#4.1) Use function declarations instead of function expressions
  
  ```javascript
  function driveBatmobile() {
  
  }
  ```
  
  - [4.2](#4.1) Format functions using correct spacing
