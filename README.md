Yet another language: Interpreted, Static-Typed, Math-Friendly, multi-arguments, Consine, High-Level, Layered(flag), Evolution-Based(flag), no-pointer, symblolic, separation of data and method, inheritance by composition, ...

Idea1: language keywords are symbols, user instructs are english

Idea2: It is layered to collaborate Architecture (API), Design (Interfaces), Implementation, Test.

Language has:
Blockes: [...] for series {...} for functions (...) for struct "", '' for text
    - which is a struct by itself and can have methods
    - subclass of error and none
Operators: >, <, >=, <=, ==, =, :=, :, /, ., ,, +, -, |, &,  *, ^, ->, ~, @, 
prefix: ?, !, ~, #, $, %, ^, \ 
types: Bit/Boolean: ~, Integer/Categories/Word: !, String: $, Bytes: \, Number: #, Generic: ?
Line Comment: %
Block Comment: %" something"
math operators: <, >, +, -, /, *, &, |, =, @ member
operator: ., ,, @, :, ; 

Anything starts with an operator is an operator, anything starts with a prefix is a prefix, and operators and prefix can not have anything else

Programmers can not use symbols (except _) for anything but operators and prefixes.

x: Int varaible decleration
x: Int = 10 Variable decleration with default
#x:= 10 The same
x:= "Alan" Constant x
x: (#) 
#x Variable x is number

(X): (a: int, b: str, c= "Alan") struct decleration
(X): (#a, $s, $c:="Alan")

(Y): (X, c: int, d: str) struct with inheritance
(Y): (X, #c, $d)

(X): (int, str) tuple decleration == (0: int, 1: str)

{f}: (...)==>(...) function decleration
(X).{f}: (...)==>(...) method decleration
(X): (key: str)==>(value: int) dictionary decleration
(X): (key: str)==>(value: none) set decleration
(X): [x: int](a: num, b: num, c: str) table deleration
(X): [](a: num)
(X): [10][5](a: num) marix 



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



- Language semantic
- Symbols define
    - [] Array: has order, no name, has duplicates, open-ended
    - () Tuple: has order or name, closed-ended, has duplicates
    - <> Set: no order or duplicate, open-ended 
    - {} Closure/dictionary: open-ended, separated by;, key: value, 
    -

Type hierarchy:
None:
    Cell: Str, Num (float), Ord (int), Bool, Byte
        - Can be copied or embeded, no inheritance, as is, no error 
    Homo: Vector, Dict {}, Set <>, List [], Tuple ()
        - Has header with error, can be pointed to
    Animal: Struct, Table, Class, 
        - Can be embeded
