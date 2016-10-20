namespace
=========

All the following type/functions names will be prefix using a namespace define by the project name. Here we will use "style" 

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

Constante (macros) + enum
==================

all in upper snake case
	
example
-------

```C
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

