# Naming

## General Naming Rules
In general, naming should be understandable to the reader. Take priority of readability over length of the name.
Do not use abbriviations unless it is known within the team or understanable from the context. Declaring variables that abbreviate the type name are alright.

## File Names
filenames should be camelCase with underscores separating components of the name.
```c++
myCatagory_myName.cc
```

## Type Names
Types should all be written in `PascalCase`.

## Variable Names
Variable names should be written in `camelCase`.
```c++
std::string tableName;
int tableLength;
```
Anything otherwise standard you should continue to use (`i, j, k...` for loop iteration, `n, o, p...` for storing an numbers for math).

## Constant Names
Variables declared with const whose value is fixed for the duration of the program should be named with the identifier `k` followed with the `PascalCase` name. You can use underscores as seperators to replace `.` in version names for example.
```c++
const int kDaysInWeek = 7;
const int kAndroid8_0_0 = 24;
```

## Function/Method Names
Function and method names are all in `PascalCase` including getters and setters
```c++
AddTableEntry()
GetCount()
SetCount()
```

## Enumerator Names
Enumerators should be named like constants, therefore, using `k` followed by the `PascalCase` name.
```c++
enum class UrlTableError {
  kOk,
  kOutOfMemory,
  kMalformedInput
}
```

## Macro Names
Macros should be easily identifiable, that is why they are names in all uppercase and with underscores
```c++
#define WHITE 13
#define PI_ROUNDED 3.0
```

## Exceptions to Naming Rules
If you are writing something that is analogous to an existing C++ entity, follow the existing naming scheme
```c++
my_hash_map //Follows STL naming conventions
```

## Comment Style
Single line comments should use `//` unless following consistency of other code.
Multi-line comments should ALWAYS use `/* */` on seperate lines to your comments.
```c++
// This is my single line comment

/*
This is my
multi-line comment
*/
```
Make sure to do your own text wrapping in a multi-line comment so that your comments do not extend past surrounding code.
