# Knowledge Center Javascript Style Guide

## Table of Contents

1. [Objects](#objects)
2. [Arrays](#arrays)
3. [Strings](#strings)
4. [Functions](#functions)
5. [Variables](#variables)
6. [Performance](#performance)

## Objects

- [1.1](#1.1) Use the literal syntax for object creation.

    ```javascript
    var batman = {};
    ```

- [1.2](#1.2) Use dot-notation when accessing properties directly.

    ```javascript
    var id = batman.secretIdentity;
    ```

- [1.3](#1.3) Use square-bracket notation when accessing properties with a variable.

    ```javascript
    var id = batman[secretIdentity];
    ```

## Arrays

- [2.1](#2.1) Use the literal syntax for array creation

    ```javascript
    var utilityBelt = [];
    ```

## Strings

- [3.1](#3.1) Use single quotes `''` for strings.

    ```javascript
    batman.secretIdentity = 'Bruce Wayne';
    ```

## Functions

- [4.1](#4.1) Use function declarations instead of function expressions.

    ```javascript
    function driveBatmobile() {
        \\ ...
    }
    ```

- [4.2](#4.1) Format functions using correct spacing

## Variables

- [5.1](#5.1) Always use ```var``` to declare variables. Write code that keeps the global namespace clean.

    ```javascript
    var superPower = new SuperPower();
    ```

- [5.2](#5.2) Declare all variables at the top of your function before you assign them. Write code the respects hoisting.

    ```javascript
    function throwBatarang() {
        var batarang;
        \\ ...
        batarang = 10;
        \\...
    }
    ```

## Performance

- [6.1](#6.1) Store the length first to improve performance when iterating through an array.

    ```javascript
    var utilityBelt = [];
    var utilityCount = arr.length;
    for(var i = 0; i < utilityCount; i++) {
        \\ ...
    }
    ```
