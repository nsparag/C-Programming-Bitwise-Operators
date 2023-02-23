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
