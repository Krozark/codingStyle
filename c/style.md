namespace
=========

All the following type/functions names will be prefix using a namespace define by the project name. Here we will use "style"

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
#ifndef style_FUNCTIONS_H
#define style_FUNCTIONS_H

#ifdef __cplusplus
extern "C"
{
#endif

	void style_funstion();

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

	void style_funstion()
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
	
void style_myFunction(int);
	
struct
======

Name are in CamelCase and suffix with _t
	
example
--------

```C
structstyle_MyStructName_t
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
typedef style_MyStructName_t style_MyStructName;
```

const +  macros + enum
==================

all in upper snake case
	
example
-------

```C
#define style_PI 3.1415 
#define style_THIS_IS_A_MACRO(x)
```

enum values
===========

all in upper snake case prefixed with the enum name the enum should also contain a special value named SIZE at the end.
	
	
example
-------

```C
enum style_MY_ENUM
{
	style_MY_ENUM_VALUE_1,
	style_MY_ENUM_VALUE_2,
	style_MY_ENUM_VALUE_3,
	style_MY_ENUM_SIZE
};
```

