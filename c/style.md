namespace
=========
	all the following type/functions names will be prefix using a namespace define by the project name. Here we will use "style" 

functions
========
	name are in camelCase
	
	example:
	--------
	
	void style_myFunction(int);
	
struct
======
	name are in CamelCase and suffix with _t
	
	example:
	--------
	
	structstyle_MyStructName_t
	{
		//...
	};

	
typedef
========
	upper CamelCase name
	
	example:
	--------
	
	typedef style_MyStructName_t style_MyStructName;


Constante (macros) + enum
==================

	all in upper snake case
	
	example:
	========
	
	#define style_THIS_IS_A_MACRO(x)
	
enum values
===========

	all in upper snake case prefixed with the enum name
	the enum should olso contain a special value named <enum name>_SIZE at the end.
	
	
	example:
	========
	
	enum style_MY_ENUM
	{
		style_MY_ENUM_VALUE_1,
		style_MY_ENUM_VALUE_2,
		style_MY_ENUM_VALUE_3,
		style_MY_ENUM_SIZE
	};

