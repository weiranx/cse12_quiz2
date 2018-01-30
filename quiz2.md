## What is a void pointer?
a pointer to everything

## What can't you do with a void pointer?
dereference

## A function call is implemented via what stack operation to the run-time stack? 
push 

## Returning from a function is implemented via what stack operation to the run-time stack? 
pop

## Besides not knowing how much memory you need, what the other main situation discussed in class when you must dynamically allocate memory in C and C++? 


## In C and C++, what is the number value of false? 
0

## In C and C++, what is the number value of true? 
1

## In C and C++, what is the number value of NULL? 
0

## In what section of memory do local variables exist? 
## In what section of memory do parameters exist? 
RTS

## In what section of memory do static variables exist?
Data

## What is the return type of "malloc"? 
void pointer

## What is the type of the parameter to "free"?
any type of pointer

## How does the parameter to "free" relate to the return value of "malloc"? 
same

## What is the unit of allocation for the parameter sent to "malloc"? 
byte

## What is the method call to give back memory allocated in C? 
free

## A "stack" data structure has the property: First In _____ _____ 
Last out

## A "stack" data structure has the property: Last In _____ _____
First out


## What keyword is used to dynamically allocate memory in Java and C++? 
new

## What keyword is used to dynamically deallocate memory in C++? 
delete

## stderr is used to display what two kinds of messages: 
debut error


## Write a function with the purpose of assigning a long that exists elsewhere to 0. 
void func(long * lp) {
  *lp = 0;
}

## Write a function with the purpose of assigning a long pointer that exists elsewhere to 0. 
void func2(long ** lpp) {
  *lpp = 0;
}

## Write a main function that has a function call to assign a local long variable to 0.
main() {
  long lll;
  func(&lll);
}


## Write a main function that has a function call to assign a local long pointer variable to 0.
main() {
  long * lp;
  func2(&lp);
}


## Are the following two types the same or different?
pointer to pointer to long
same

## pointer to long pointer
same

## Showing variable names, known memory addresses and including arrows where appropriate, draw the RTS showing a main method with a local long variable, lll, calling a method that assigns lll to 0. The name of the parameter is lp. The address of lll is 1000. 


## Showing variable names, known memory addresses and including arrows where appropriate, draw the RTS showing a main method with a local long pointer variable, lp, calling a method that assigns lp to 0. The name of the parameter is lpp. The address of lp is 1000.

## Showing variable names, known memory addresses and including arrows where appropriate, draw the RTS for: void func (long * lp) { *lp = 0; } main() { long * lp; func (lp);} The address of lp in main is 1000.

## What is the type of 0? 
all types

## Is 0 of type void pointer? 
yes

## Is 0 of type int pointer?
yes

## In the expression: xzy = sizeof (Stack); is sizeof (Stack) a typical function call?
no

## Excluding validity checks and return values, write the body code for the push function of hw3. 
'
long sp = this_Stack[SPI];
this_Stack[sp] = item;
this_Stack[SPI]++;
'

## Excluding validity checks and return values, write the body code for the pop function of hw3. 
'
long sp;
sp = --this_Stack[SPI];
*item = this_Stack[sp];
'


## Excluding validity checks and return values, write the body code for the top function of hw3.
'
long sp = this_Stack[SPI];
*item = this_Stack[sp-1];
'


## Excluding validity checks and return values, write the body code for the empty_Stack function of hw3. 
'
this_Stack[SPI] = 0;
'
## What condition is checked to determine if the stack is empty in hw3? 
stack pointer index == 0

## What condition is checked to determine if the stack is full in hw3?
spi == stacksize index

## What are the two responsibilities of the delete_Stack function of hw3? 
deallocate; assign the pointer to 0

## What are the two responsibilities of the new_Stack function of hw3?
allocate stack; init stack count, stack size

## What is the Object-Oriented term describing each of a collection of functions defined within the same file in C each with a common first parameter? 
member methods

## What is the Object-Oriented term describing the new_Stack method of hw3? 
constructor

## What is the Object-Oriented term describing the delete_Stack method of hw3?
destructor

## Translate the following method call using your hw3 stack into an equivalent line of Java code assuming needed classes and variables are defined.
push (mainStack, 10); /* C code */

mainStack.push(10); // Java code

## Which stack methods of hw3 need to check if the stack is full before the requested operation can be completed successfully? 
push; isfull

## Which stack methods of hw3 need to check if the stack is empty before the requested operation can be completed successfully?

## In the push function, what is the name and type of the first parameter? 
Stack pointer

## In the pop function, what is the name and type of the first parameter? 
stack pointer 

## In the top function, what is the name and type of the first parameter?

## When calling free, is the caller giving up access to or authority to access memory or both? 
authority

## When assigning a pointer to null, is the caller giving up access to or authority to access memory or both? 
access

## In C, what are the three illegal kinds of declarations?
array of functions; returning functions; 

## With parallel arrays, two or more arrays share the same ________ 
index

## In C, in what kind of file do you list public information? 
.h

## In C, in what kind of file do you list private information? 
.c

## In C, in what kind of file do you list hidden information?
.c

## Generally speaking, what goes in a .h file? (an answer of declarations and type definitions is too specific) 
public information

## Name the three binary masking bit manipulation operations
| & ^


## Intuitively speaking, ANDing with ones gives ____________ 
the same

## Intuitively speaking, ANDing with zeros gives ____________
zeros

## Intuitively speaking, ORing with ones gives ____________ 
ones

## Intuitively speaking, ORing with zeros gives ____________
the same

## Intuitively speaking, XORing with ones gives ____________ 


## Intuitively speaking, XORing with zeros gives ____________

## What is the English word to describe XORing with one continuously? 
toggle

## XORing a value with itself gives ___________
zero

## In 8 bits, what is the result of ~01010101? 
flip

## In 8 bits, what is the result of 01010101 & 00001111? 
00000101

## In 8 bits, what is the result of 01010101 | 00001111? 
01011111

## In 8 bits, what is the result of 01010101 ^ 00001111?
01011010

## How do you describe the result of the following three operations?
xxx ^= yyy; yyy^=xxx; xxx^=yyy;
swap
xxx: 10101010
yyy: 11110000
xxx: 01011010   xxx = xxx ^ yyy
yyy: 10101010   yyy = xxx ^ yyy
xxx: 11110000   xxx = xxx ^ yyy
swap x and y without temp

## T or F: ANDing is used to extract bits. 
T

## T or F: ANDing is used to set bits. 
F

## T or F: ANDing is used to clear bits. 
T

## T or F: ANDing is used to flip bits.
F

## T or F: ORing is used to extract bits. 
F

## T or F: ORing is used to set bits. 
T

## T or F: ORing is used to clear bits. 

## T or F: ORing is used to flip bits.

## T or F: XORing is used to extract bits. 
F
## T or F: XORing is used to set bits. 
## T or F: XORing is used to flip bits.

## Shifting bit to the right has the effect of ___________ 
divide by power of two

## Shifting bit to the left has the effect of ___________
multiply 2
## What is the operator used to shift bits to the left? 
<<

## What is the operator used to shift bits to the right?
>>

## In your calculator of hw4, what is the best word to describe the character that intopost will "unget"? 
digits

## In your calculator of hw4, what is the best word to describe the character that decin will "unget"?
non digits

## In your intopost code of hw4, the values pushed to a stack originate from what two functions?
setupword(); decin()


Using English words, describe the following declaration:
int (*x)[][];


Using English words, describe the following declaration:
int (*x)()[];

Using English words, describe the following declaration:
int (*x[])();

Using English words, describe the following declaration:
int x[][]();

Using English words, describe the following declaration:
int (*x())[];

Using English words, describe the following declaration:
int x()[]();

Using English words, describe the following declaration:
int *(*x)[];

Using English words, describe the following declaration:
int (*x())();

Using English words, describe the following declaration:
int (*x[])[];

Using English words, describe the following declaration:
long (*x[])(long,long);
array of pointers to functions taking two longs returning long

## Considering a tiered or layered design, each method need to work based on its ________ and ________ values. 
params; return values

## T or F: Considering a tier or layered design, methods of outer tiers are called by methods of inner tiers. 
F

## T or F: Considering a tier or layered design, methods of inner tiers are called by methods of outer tiers.
T

## Assuming malloc returned 2000, draw a hw3 stack created with a size of 10 after pushing 25, 50, 75, 100 and popping twice.
pop 

