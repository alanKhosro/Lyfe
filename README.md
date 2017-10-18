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
- Operator, binary and unary 


alternative notation:
- [](int ==> str) for dictionary
- [](==>str) set
- [](int) for array
- [](interface) for list
- (i int, s str) for tuple or (int, str)
- [5, 6](int) matrix
- [9](int) vector
- [label int](col1 num, col2 str, col3 str) table

exaample
a = [](int ==> str ==> table)
a[5] 
a[5]['Alan']
a[5]['Alan'][8](col1, col2) 
for x in a[5]['Alan'][x](col1) {
 ### do something
}





A: <a int, b []int, C, d D> -> <f, g, h>

Type hierarchy:
None:
    Cell: Str, Num (float), Ord (int), Bool, Byte
        - Can be copied or embeded, no inheritance, as is, no error 
    Homo: Vector, Dict {}, Set <>, List [], Tuple ()
        - Has header with error, can be pointed to
    Animal: Struct, Table, Class, 
        - Can be embeded
