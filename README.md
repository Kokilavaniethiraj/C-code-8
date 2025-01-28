# C-code-8
Pascal Triangle Pattern in C language

#include <stdio.h>

int main()
{
    int n;
    scanf("%d",&n);
    for(int i=0;i<=n;i++){
        for(int s=0;s<=n- 1-i;s++){
            printf(" ");
        }
        int num=1;
        for(int j=0;j<=i;j++){
            printf("%d ",num);
            num=num*(i-j)/(j+ 1);
        }
        printf("\n");
    }
    return 0;
}
