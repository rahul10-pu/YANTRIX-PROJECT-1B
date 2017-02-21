	

Project 1A: Stacks and Queues

Project partners-This is a individual Project.

Submission. Your completed project should be uploaded on Github. A Readme file with complete directions on use of the application, installation instructions, a specific step-by-step walk-through, and any application dependencies, if applicable. An executable application file or software package for your solution.

Project A- Matching Brackets. Complete a program that performs the bracket matching task. Your program will prompt the user for an input string, and then output whether the string has properly-matching brackets.
Roughly speaking, brackets are properly matched in a string of text if:
1. every opening bracket has its own corresponding closing bracket, 2. every closing bracket corresponds to an opening bracket, and
3. no opening bracket reaches its corresponding closing bracket until all the opening brackets coming after it have already been closed.

The formal definition of whether a string’s brackets are matched can be derived from the pseudocode for the algorithm which we will discuss in class.

As we will discuss in class, a simple way to solve this problem is to use a stack. Therefore, you will need to implement a Stackclass/function, with its standard fields and methods. You may choose whether to implement an array-based stack or a linked-list-based stack. You can test that your stack operations are working properly from a main method (used just for testing) within your stack class/function.
To solve this Bracket Matching problem, you will also implement the following classes:

	The BracketMatchAppclass. (Only contains a main method, no fields or other methods.)
	the mainmethod: /* drives the user input/output of the program */
	prompt user for input string output whether or not the string has its brackets matched properly.	
	The BracketMatcherclass.
	Fields:

•	hard-coded array of characters (of type char) holding the opening brackets (these should include: ‘(‘, ‘[‘, ‘{‘, ‘<’).
•	hard-coded parallel array of characters (of type char) holding the closing brackets.


Methods:
•	boolean isOpeningBracket(char c)
	returns trueiff the character cis an opening bracket
•	boolean isClosingBracket(char c)
	returns trueiff the character cis a closing bracket
•	boolean corresponds(char open, char close)
	returns trueiff the character openis a bracket that corresponds to the closing bracket character close
	note that we set up parallel arrays of brackets to help us with this task
•	boolean checkBrackets(String s)
	returns trueiff the string shas brackets that are all matched up properly
	calls the other three methods to achieve this.
