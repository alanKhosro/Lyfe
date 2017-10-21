# Zan
Yet another language: Interpreted, Static-Typed, Math-Friendly, separation of data and functions, consine, High-Level, Layered, symbolic 

Idea1: all language literals are symbols.

Idea2: It is layered to collaborate Architecture (API), Design (Interfaces), Implementation, Test. 

Prime Types with their defaults (None): {
    Number: #
    Bit/Boolean: ?
    Integer/Categories/Word: !
    String: _
    Bytes: [`]   `
}
Commenting: `a`
Blockes:
[...] for series
{...} for functions
(...) for struct
"", '' for text

Operators:
Math: <, >, +, -, /, *, &, |, // redical, ** power, =, - negation, @ member, subset <, << strict, >>, 
operator: ., ,, @, :, ;
prefix: ?, !, ~, _, #, $, %, ^, \
postfix: ?, !, ;

Language has:
- Blocks: [...] series, {...}, (...), "...", '...'
    - which is a struct by itself and can have methods
    - subclass of error and none
- Operators: >, <, >=, <=, ==, =, :=, :, /, ., ,, +, -, |, &,  *, ^, ->, ~, @, <>
- prefix: ?, !, #, $, %, \
- types: (bit), (byte), (word), (str), num, int, complex, none, zero, error



- Math like 
    - A.f: (a int=0, s str, d {int, int}) -> (i int) {

    }

(X): #
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
