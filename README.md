# Knowledge Center Javascript Style Guide

## Table of Contents

  1. [Objects](#objects)

## Objects

  - [1.1](#1.1) Use the literal syntax for object creation.

    ```javascript
    // bad
    var obj = new Object();

    // good
    var obj = {};
    ```
  
  - [1.2](#1.2) Use dot-notation when accessing properties directly
  
    ```javascript
    var bar = foo.bar;
    ```
  - [1.3](#1.3) Use square-bracket notation when access properties with a variable
  
    ```javascript
    var bar = foo[bar];
    ```
