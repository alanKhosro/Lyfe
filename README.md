# Zan
Yet another language: Interpreted, Static-Typed, Math-Friendly, Functional, Weak OO, Brief, High-Level, Layered, Evolution-Based 


Specs of a new language:
- Interpreter
- Static typed
- Concine and brief
- Easy to read
- Separation of data and behavior 
- Math like 
    - A.f: (a int=0, s str, d {int, int}) -> (i int) {

    }

- Language semantic
- Symbols define
    - [] Array: has order, no name, has duplicates, open-ended
    - () Tuple: has order or name, closed-ended, has duplicates
    - <> Set: no order or duplicate, open-ended 
    - {} Closure/dictionary: open-ended, separated by;, key: value, 
    -
Language has:
- Blocks: [...], {...}, (...), "...", '...'
    - which is a struct by itself and can have methods
    - subclass of error and none
- Operators: >, <, >=, <=, ==, =, :=, :, /, ., ,, +, -, |, &,  *, ^, ->, ~, @, <>
- prefix: ?, !, #, $, %, \
- types: (bit), (byte), (word), (str), num, int, complex, none, zero, error
- function

{f}: (...)==>(...) function decleration
(X): (...) struct decleration
(X): (int) struct decleration
(X).{f}: (...)==>(...) method decleration
(X): [x: int][y: str](int) matrix decleration
(X): (ticker: str)==>(report: str)==>[x: int](col1: str, col2: str, col3: num) Dictionary of dictionary of Table decleration
(X): (ticker: str)==>(report: str)==>(col1: [row: int]str, col2: [row]str, col3: [row]num) dataframe decleration
(X): (ticker: str)==>(report: str)==>(col1: []str, col2: []str, col3: []num) R list decleration
(X): [a: str](b: int)

[x]: (int) list of int decleration
[x]: (X) list of (X) decleration
[x]: (a int, b str) list of struct decleration (table)
[x]: (key: int) ==> (value: str) dictionary decleration
[x][y]: int matrix of x,y decleration


x: (0<x<10)
x: (int) variable decleration
x: () generic decleration
a: [x][y]

x= [1,2] 
x= 10
f= {...} function implementation




alternative notation:
- [](int ==> str) for dictionary
- [](==>str) set
- [](int) for array
- [](interface) for list
- a=(int, str) for tuple == (0 int, 1 str)
- (i int, s str, a) for struct and inheritance
- (i int, s str) for tuple or (int, str)
- [5, 6](int) matrix
- [9](int) vector
- [label int](col1 num, col2 str, col3 str) table

example
a = (
a = [](ticker ==> report ==> table)
a[5] 
a[5]['Alan']
a[5]['Alan'][8](col1, col2) 
{
 ### do something
}.for(x: a[5]['Alan'][x](col1)) 

{
#statements
}.for(key,value: a[key][value][]()
{
#statements
}.for(x: 0<x<10)

{
#statements
}.while(bool expressions, initial condition, step)

{
#statements
}.until(bool expression, initial condition, step)

[].

A: <a int, b []int, C, d D> -> <f, g, h>

Type hierarchy:
None:
    Cell: Str, Num (float), Ord (int), Bool, Byte
        - Can be copied or embeded, no inheritance, as is, no error 
    Homo: Vector, Dict {}, Set <>, List [], Tuple ()
        - Has header with error, can be pointed to
    Animal: Struct, Table, Class, 
        - Can be embeded
