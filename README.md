# FACTORIAL-OF-A-NUMBER

---

## APPARATUS REQUIRED
- Personal computer with Keil software

---

## ALGORITHM
1. *Start*
2. *Input*: Read the number n.
3. *Initialize*:
   - Set factorial to 1.
   - Set i to 1.
4. *Loop*: While i is less than or equal to n:
   - Multiply factorial by i.
   - Increment i by 1.
5. *Output*: Store or print the value of factorial.
6. *End*

---

## FLOWCHART
<img width="506" height="525" alt="image" src="https://github.com/user-attachments/assets/f3b47187-6f0f-490c-8704-f2973cb2b276" />


---

## PROGRAM

ORG 000H
MOV DPTR,#4500H
MOVX A,@DPTR
MOV R0,A
INC DPTR
ACALL FACTORIAL
MOVX @DPTR,A
SJMP THIN
FACTORIAL:DEC R0
CJNE R0,#01H,PRODUCT
SJMP THICK
PRODUCT:MOV B,R0
MUL AB
ACALL FACTORIAL
THICK: RET
THIN:RET
END



## OUTPUT
<img width="1919" height="1079" alt="Screenshot 2025-09-24 084743" src="https://github.com/user-attachments/assets/32bbf33a-b3db-458b-adf9-f25fdf98820d" />


---

## MANUAL CALCULATIONS
![105f2a45-76cc-46d9-9749-97cb66be68ab](https://github.com/user-attachments/assets/dfa4f6d0-f734-4aef-b323-a5a7d2a03e66)

---

## RESULT

Thus, the factorial of a number was calculated and executed successfully using 8051 Keil.

---
