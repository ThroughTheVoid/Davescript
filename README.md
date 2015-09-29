# RCScript

An interpreted language implemented in C.

## Build

Compiled with MinGW for Windows
http://www.mingw.org/

## Goal

Interpret a basic hello world / read input / if statement program such as

'''

name = input()

print("Hello " + name)

if name == "Dave" then
	print("Which Dave?")
end

'''

etc.

## Planned Features
* Basic Math
* Variables
* If Statements
* Key Input

## Algorithm
* Convert String to Tokens
ex. "2+4*32" -> {2,'+',4,*,32}
* Check If Tokens Are a Valid Expression
ex. { 2, '/', 0 } should be resolved as invalid.
* Evaluate Parenthesis (Convert To Tree?)
ex. (2+4) of 1+(2+4)*3 should be resolved somehow (not sure about this yet)
