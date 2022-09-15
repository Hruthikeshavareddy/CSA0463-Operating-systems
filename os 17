#include <stdio.h>
#include <stdlib.h>

int main(int argc, char** argv)
{
    int id = 0, err = 0;
    int* mem; 
    if (id == -1)
        perror("shmget");
    else
        printf("Allocated with shm id %d\n", (int)id);

        perror("shmat");

    *mem = 100; 
    printf("Start other process-->");
    getchar();
    printf("mem is now %d\n", *mem);

    if (err == -1)
        perror("shmctl");
    else
        printf("Removed %d\n", (int)(err));


    return 0;
}
