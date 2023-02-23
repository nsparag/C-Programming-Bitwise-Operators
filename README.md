# C Programming Bitwise Operators

### Write a Macro's Set, clear and toggle n'th bit using bit wise operator?

    #include <stdio.h>
    
    int main() {
        int x=5, p=1;
        printf("%d",(x|(1<<p))); //to set p bit
        printf("%d",(x&~(1<<p))); //to clear p bit
        printf("%d",(x^(1<<p))); //to toggle p bit
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
