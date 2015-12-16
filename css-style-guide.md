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
9. [Quotation Marks](#quotation-marks)


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

## Hexidecimal Notation
- [3.1](#3.1) Use lowercase and shorthand hex values, e.g., <code>#aaa</code>.

## Units After 0
- [4.1](#4.1) Avoid specifying units for zero-values, e.g., <code>margin: 0</code>.

## Declaration Order
- [5.1](#5.1) Alphabetize declarations.</li>

## Declaration Stops
- [6.1](#6.1) Include a semi-colon at the end of every declaration</li>

## Property Name Stops
- [7.1](#7.1) Include a single space after the colon of a property.</li>

## Rule Separation
- [8.1](#8.1) Separate each ruleset by a blank line.</li>

## Quotation Marks
- [9.1](#9.1) Use double quotes e.g., <code>content: ""</code>.</li>
- [9.2](#9.2) Quote attribute values in selectors, e.g., <code>input[type="checkbox"]</code>.</li>
