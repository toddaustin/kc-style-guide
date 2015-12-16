# Javascript Style Guide

## Table of Contents

1. [Objects](#objects)
2. [Arrays](#arrays)
3. [Strings](#strings)
4. [Functions](#functions)
5. [Variables](#variables)
6. [Comparison Operators](#comparison-operators) 
7. [Comments](#comments)
8. [White Space](#white-space)
9. [Semicolons](#semicolons)
10. [Naming Conventions](#name-conventions)
11. [jQuery](#jquery)
12. [Performance](#performance)

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

- [3.1](#3.1) Use single quotes ```''``` for strings.

    ```javascript
    batman.secretIdentity = 'Bruce Wayne';
    ```

## Functions

- [4.1](#4.1) Use function declarations instead of function expressions.

    ```javascript
    function driveBatmobile() {
        // ...
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
        // ...
        batarang = 10;
        // ...
    }
    ```

## Comparison Operators

- [6.1](#6.1) Use ```===``` and ```!==``` instead of ```==``` and ```!=```.

    ```javascript
    if(id === 'Bruce Wayne') {
        // ...
    }
    ```

- [6.2](#6.2) Use shortcuts.

    ```javascript
        if(isBatman) {
            // ...
        }
        
        if(utilityBelt.length) {
            // ...
        }
    ```

- [6.3](#6.3) Place your ```else if``` and ```else``` on the same line as your ```if``` closing brace.

    ```javascript
    if(isBatman) {
        // ...
    } else {
        // ...
    }
    ```

## Comments

- [7.1](#7.1) Use ```/** ... */``` for multi-line comments. Write descriptively.

    ```javascript
    /**
    * Return an array of the superHero's super power
    */
    function getSuperPower(superHero) {
        // ...
    }
    ```

- [7.2](#7.2) Use ```//``` for single line comments. Place single line comments on a new line above the subject of the comment. Put an empty line before the comment unless it's on the first line of a block.

    ```javascript
    function getSuperPower(superHero) {
        // set default super power
        var superPowers = false;
        
        // get array of super powers
        superPowers = superhero.superPower;
        
        return superPowers;
    }
    ```

## Whitespace

- [8.1](#8.1) Indent using 4 spaces.

    ```javascript
    function() {
        var superPower;
    }
    ```

- [8.2](#8.2) Place 1 space before a leading brace.

    ```javascript
    function() {
        // ...
    }
    
    superHero.set('attr', {
        superHeroIdentity: 'Batman',
        secretIdentity: 'Bruce Wayne'
    });
    ```

- [8.3](#8.3) Place 1 space before the opening parenthesis in control statements (```if```, ```while``` etc.). Place no space before the argument list in function calls and declarations.

    ```javacript
    if(isBatman) {
        var superPowers = getSuperPower(batman);
        alert(superPowers);
    }
    ```

- [8.4](#8.4) Place 1 space between operators.

    ```javascript
    var x = y + 5;
    ```

- [8.4](#8.4) Do not add spaces inside parentheses.

    ```javascript
    function getSuperPower(superHero) {
        // ...
    }
    ```

- [8.5](#8.5) Do not add spaces inside brackets.

    ```javascript
    var utilityBelt = [batarang,bathook,kryptonite];
    console.log(utilityBelt[0]);
    ```

- [8.6](#8.6) Add spaces inside curly braces.

    ```javascript
    var batman = { secretIdentity: 'Bruce Wayne' };
    ```

## Semicolons

- [9.1](#9.1) ***Yes.***

    ```javascript
    function() {
        var secretIdentity = 'Bruce Wayne';
        return secretIdentity;
    }
    ```

## Naming Conventions

- [10.1](#10.1) Avoid single letter names. Be descriptive with your naming.

    ```javascript
    // this is bad naming
    var n = 'Bruce Wayne';
    
    // this is good, descriptive naming
    var secretIdentity = 'Bruce Wayne';
    ```

- [10.2](#10.2) Use camelCase when naming objects, functions, and instances.

    ```javascript
    var secretIdentity = 'Bruce Wayne';
    var batman = {};
    
    function driveBatmobile() {
        // ...
    }
    ```

- [10.3](#10.3) Use PascalCase when naming constructors or classes.

    ```javascript
    var superPower = new SuperPower();
    ```

## jQuery

- [11.1](#11.1) Prefix jQuery object variables with a ```$```.

    ```javascript
    var $search = $('.search');
    ```

## Performance

- [12.1](#12.1) Store the length first to improve performance when iterating through an array.

    ```javascript
    var utilityBelt = [];
    var utilityCount = arr.length;
    for(var i = 0; i < utilityCount; i++) {
        // ...
    }
    ```

- [12.2](#12.2) Store jQuery lookups if you are using it more than once.

    ```javascript
    var $search = $('.search');
    $search.hide();
    // ...
    $search.show();
    ```
