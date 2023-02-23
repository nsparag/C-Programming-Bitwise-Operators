# C Programming Bitwise Operators

### Write a Macro's Set, clear and toggle p'th bit using bit wise operator?

    #include <stdio.h>

    #define SET(x,p) x|=(1<<p)
    #define CLEAR(x,p) x&=~(1<<p)
    #define TOGGLE(x,p) x^=(1<<p)
    int main() {
        int x=5, p=1;
        SET(x,p);
        printf("%d",x); //to set p bit

        CLEAR(x,p);
        printf("%d",x); //to clear p bit

        TOGGLE(x,p);
        printf("%d",x); //to toggle p bit
        return 0;
    }
    
### Write a program to print binary of decimal number.

    #include <stdio.h>

    int main() {
        int x=16,y[10],count=0,i;
        while(x!=0)
        {
        y[count]=x%2;
        x=x/2;
        count++;
        }
        for(i=count-1;i>=0;i--)
            printf("%d",y[i]);
    }

## Multiply a mumber by 9
    #include <stdio.h>

    int main() {
        int x=3,y;
        y=x<<4-x<<2;
        printf("%d",y);

        return 0;
    }
    
    
## Write a program to count the number of 1's in an integer?

    #include <stdio.h>

    int main() {
        int num=7,flag=0;
        while(num!=0)
        {
            if(num&1)
                flag++;
            num=num>>1;
        }
        printf("%d",flag);
        return 0;
    }

4. WAP implement subtraction functionality with out using SUB('-') Operator.    
5. WAP implement addition functionality with out using ADD('+') Operator.   
6. WAP implement XOR functionality with out using XOR(^) operator.
7. WAP to implement the sizeof operation using the bitwise operator.  
8. WAP to convert Little endian integer to Big endian integer 
9. WAP multiply a number by 9 using bit shift.
10. WAP whether a number is ODD or EVEN using bitwise.
11. WAP whether a number is a power of 2 or not?
12. WAP print reverse of integer number? 
13. WAP Check if the 20th bit of a 32-bit integer is on or off?
14. Write a functionsetbits(x,p,n,y)that return x with then bits that begin at position p set to the rightmost n bits of y, leaving the other bits unchanged.
e.g. if x = 10101010 (170 decimal) and y = 10100111 (167 decimal) and n = 3 and p = 6 then
you need to strip off 3 bits of y (111) and put them in x at position 10xxx010 to get answer
10111010. Your answer should print out the result in binary form although input can be in
decimal form.
Your output should be like this:
x = 10101010 (binary)
y = 10100111 (binary)
setbits n = 3, p = 6 gives x = 10111010 (binary).

15. WAP Swap any two numbers using bitwise operators. How does it work?
