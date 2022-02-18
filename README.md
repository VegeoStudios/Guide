# Naming

## General Naming Rules
In general, naming should be understandable to the reader. Take priority of readability over length of the name.
Do not use abbriviations unless it is known within the team or understanable from the context. Declaring variables that abbreviate the type name are alright.
Name length should be proportional to the scope. For example, global variables should have a descriptive name to make sure it is clear what the purpose is.
```c++
double sqrt(double x);
int length(const char* p);

int lengthOfString(const char zeroTerminatedArrayOfChar[])    // bad: verbose

int g;      // bad: global variable with a cryptic name
int open;   // bad: global variable with a short, popular name
```

## File Names
filenames should be `camelCase` with underscores separating components of the name.
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

## Constant Names
Variables declared with const whose value is fixed for the duration of the program should be named in all caps with underscores.
```c++
const int DAYS_IN_WEEK = 7;
const int ANDROID8_0_0 = 24;
```

## Function/Method Names
Function and method names are all in `camelCase` including getters and setters
```c++
addTableEntry()
getCount()
setCount()
```

## Enumerator Names
Enumerators should be named like constants.
```c++
enum class UrlTableError {
  OK,
  OUT_OF_MEMORY,
  MALFORMED_INPUT
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

