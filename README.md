# LC3-Machine-Language

## What is LC3?
LC3 stands for "Little Computer 3" and is a basic machine language standard commonly used for educational purposes.  More info can be found here: https://en.wikipedia.org/wiki/Little_Computer_3

## Program 1
This program loops X times, incrementing a counter each time it loops.  The value of X is stored in memory and is indirectly accessed [using the load indirect instruction]. The program starts at x3000.  Additionally, x3020 contains the address (x30A0) for the value of X [which is x000F].

## Program 2
This program compares two values stored at memory locations x30A2 and x30A3.  If the value at x30A2 is larger than the value at x30A3, then the value of 1 is stored in R1.  Else, the value of 0 is stored in R1.  PC + offset addressing is used to load contents of x30A2 into R2 and x30A3 into R3.

## Program 3
Performs the same task as **Program 2**, but uses Base + offset [load register].  Uses the load immediate [LEA] instruction to set up the base [R4] with the address of x30A2.
