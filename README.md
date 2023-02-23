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
