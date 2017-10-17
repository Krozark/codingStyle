Indentation
===========

Use 4 spaces to indente and no tabs.
Moreover Allman style is used (https://en.wikipedia.org/wiki/Indentation_style#Allman_style)

namespace
=========

All the following type/functions names will be prefix using a namespace define by the project name.

files extention + content
=====

Extention are .h for header and .c for implementation.

Each header file must contain a guard as follow: 

```C
#ifndef <namespace>_FILE_IDENTIFIER_NAME_H
#define <namespace>_FILE_IDENTIFIER_NAME_H

//... code

#endif //guard
```

All function are in a extern "C" block for a library.

example
--------

functions.h
```C
#ifndef <namespace>_FUNCTIONS_H
#define <namespace>_FUNCTIONS_H

#ifdef __cplusplus
extern "C"
{
#endif

void <namespace>_function();

#ifdef __cplusplus
}
#endif

#endif
```

functions.c
```C
#include "function.h"

#ifdef __cplusplus
extern "C"
{
#endif

void <namespace>_function()
{
	// code go here
}

#ifdef __cplusplus
}
#endif
```


functions
========

Name are in camelCase
	
example
--------
	
void <namespace>_myFunction(int);
	
struct
======

Name are in CamelCase and suffix with _t
	
example
--------

```C
struct <namespace>_MyStructName_t
{
	//...
};
```

	
typedef
========
upper CamelCase name
	
example
--------

```C
typedef struct <namespace>_MyStructName_t <namespace>_MyStructName;
```

const +  macros + enum
==================

all in upper snake case
	
example
-------

```C
#define <namespace>_PI 3.1415 
#define <namespace>_THIS_IS_A_MACRO(x)
```

enum values
===========

all in upper snake case prefixed with the enum name the enum should also contain a special value named SIZE at the end.
	
	
example
-------

```C
enum <namespace>_MY_ENUM
{
	<namespace>_MY_ENUM_VALUE_1,
	<namespace>_MY_ENUM_VALUE_2,
	<namespace>_MY_ENUM_VALUE_3,
	<namespace>_MY_ENUM_SIZE
};
```

control struct (if, else, while, for, do, switch)
=================================================

All control struct must create there own block (using "{" ).
if statement are split into separate line for the test and the code to execute

switch satement must contain a default.

example
-------

```C
if (my_var == other_var)
{
	//...
}
else
{
	//...
}

while(whatever)
{
	//...
}

switch (mv_var)
{
	case 1:
	{
		//...
	}break;
	case 2:
	{
		//...
	}break;
	case 3:
	{
		//...
	}break;
	default:
	{
	}
}
```

