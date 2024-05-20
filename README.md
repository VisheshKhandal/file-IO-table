# file-IO-table
#include<stdio.h>

int main() {
    FILE *ptr;
    int num;
    printf("enter the number : \n");
    scanf("%d", &num);
    ptr = fopen("file.txt", "w");
    for(int i = 0; i < 10; i++){
        fprintf(ptr, "%d X %d  = %d\n", num , i+1,num*(i+1));  
    }
    printf("SUCCESSFULLY GENERATED YOUR TABLE OF %d TO file.txt\n",num );
    return 0;
}
