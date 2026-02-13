# SQUARE AND CUBE OF A NUMBER
# 8051 Square  Program

## AIM
To write and execute an Assembly language program for finding the square of a given data using 8051 microcontroller in Keil software.

## APPARATUS REQUIRED
- Personal computer
- Keil μVision IDE

## ALGORITHM
1. Enter the Assembly language program.
2. Provide the input value to Port 0 (P0).
3. Execute the program.
4. The output square value is stored in Port 2 (P2).

## PROGRAM
```
ORG 0000H
MOV DPTR, #8100H
MOVX A, @DPTR
MOV B,A
MUL AB
MOV DPTR, #8102H
MOVX @DPTR,A
INC DPTR
MOV A,B
MOVX @DPTR,A
END








```

## OUTPUT

<img width="818" height="224" alt="Screenshot 2026-02-13 111131" src="https://github.com/user-attachments/assets/9442b856-0310-4075-a18f-98ffe6a3096b" />


## RESULT
Thus, the square of the given data is calculated using 8051 Keil.

# 8051 Cube  Program

## AIM
To write and execute an Assembly language program for finding the cube of a given data using 8051 microcontroller in Keil software.

## APPARATUS REQUIRED
- Personal computer
- Keil μVision IDE

## ALGORITHM
1. Enter the Assembly language program.
2. Provide the input value.
3. Execute the program.
4. The output cube value is stored in a memory location.

## PROGRAM
```
ORG 0000H
MOV DPTR, #9000H
MOVX A, @DPTR
MOV B,A
MOV R1,A
MUL AB
MOV R2,B
MOV B,R1
MUL AB
MOV DPTR, #9003H
MOVX @DPTR,A
MOV R3,B
MOV B,R2
MOV A,R1
MUL AB
ADD A,R3
DEC DPL
MOVX @DPTR,A
MOV A,#00H
ADDC A,B
DEC DPL
MOVX @DPTR,A
END







```


## OUTPUT
![WhatsApp Image 2026-02-13 at 11 10 26 AM](https://github.com/user-attachments/assets/6e5396c8-4186-42f3-804a-5ed0c07735cd)


## RESULT
Thus, the cube of the given data is calculated using 8051 Keil.
