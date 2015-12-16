# CSS Style Guide

## Table of Contents

1. [Indentation](#indentation)
2. [Shorthand Properties](#shorthand-properties)
3. [Hexidecimal Notation](#hexidecimal-notation)
4. [Units After 0](#units-after-0)
5. [Declaration Order](#declaration-order)
6. [Declaration Stops](#declaration-stops)
7. [Property Name Stops](#property-name-stops)
8. [Rule Separation](#rule-separation)
9. [Selector and Declaration Separation](#selector-and-declaration-separation) 
10. [Quotation Marks](#quotation-marks)


## Indentation
- [1.1](#1.1) Indent by 4 spaces]
    
    ```css
        h2 span {
            font-size: .7em;
            font-weight: normal;
        }
    ```
- [1.2](#1.2) Use one level of indentation for each declaration.

    ```css
    @media screen, projection {
        html {
            background: #fff;
            color: #444;
        }
    }
```

## Shorthand Properties
- [2.1](#2.1) Use shorthand properties where possible

    ```css
        p {
            font: 100%/1.1 arial, helvetica, sans-serif;
            padding: 0 1em 2em;
        }
    ```

## Hexidecimal Notation
- [3.1](#3.1) Use lowercase and shorthand hex values.

    ```css
        .hoth {
            color: #fff;
        }
    ```

## Units After 0
- [4.1](#4.1) Avoid specifying units for zero-values.

    ```css
        .jawas {
            margin: 0 5px 10px 0;
        }
    ```

## Declaration Order
- [5.1](#5.1) Alphabetize declarations.

    ```css
        .dagobah {
            background: #0e3557 url(../img/yoda.png) 0 0 no-repeat;
            border-radius: 2px;
            color: #fff;
            font: 16px arial, helvetica, sans-serif;
            padding: 0;
            margin: 5px 10px;
        }
    ```

## Declaration Stops
- [6.1](#6.1) Include a semi-colon at the end of every declaration

    ```css
        .death-star {
            margin: 20px 0 0 35px;
            padding: 25px;
        }
    ```

## Property Name Stops
- [7.1](#7.1) Include a single space after the colon of a property.

    ```css
        .darth-vader {
            margin: 0;
        }
    ```

## Rule Separation
- [8.1](#8.1) Separate each ruleset by a blank line.

    ```css
        h2 {
            color: #1d3b53;
        }

        h2 span {
            font-size: .5em;
            font-weight: normal;
      }
    ```
## Selector and Declaration Separation
- [9.1](#9.1) Separate selectors and declaration by new lines

    ```css
        .stormtrooper,
        .emperor-palpatine,
        .boba-fett {
            background-color: #0e3557;
        }
    ```

## Quotation Marks
- [10.1](#10.1) Use double ("") quotation marks for attribute selectors or property values. Do not use quotation marks in URI values (url()).

    ```css
        input[type="checkbox"] {
            padding: 5px
        }
        
        .chewbacca{
             background-image: url(../img/palpatine.png);
        }
        
    ```
