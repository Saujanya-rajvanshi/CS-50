# CS-50
harvard University 

```c
#include <stdio.h>
#include <stdlib.h>

int main(void){
    int *list = malloc(3 * sizeof(int));
    list [0] = 1;
    list [1] = 2;
    list [2] = 3;
    for (int i = 0; i < 3; i++){
        printf("%i\n", list[i]);
    }
}
```
```c
#include <stdio.h>
#include <stdlib.h>

int main(void){
    int *list = malloc(3 * sizeof(int));
    
    if (list == NULL){
        return 1;
    }
    
    list [0] = 1;
    list [1] = 2;
    list [2] = 3;
    
    int *tmp = malloc(4 * sizeof (int));
    
    if (tmp == NULL){
        return 1;
    }
    
    for(int i = 0; i < 3;i++){
        tmp[i]=list[i];
    }
    tmp[3]=4;
    
    free (list)

    for (int i = 0; i < 3; i++){
        printf("%i\n", list[i]);
    }
}
```

```c
node *list ; //points to a garbage value
node *list = NULL; //points to an empty value
node *n = malloc(sizeof(node)); //allocating space for node
*n.number = 1; //putt element
n -> number = 1;
n -> next = NULL ; //put next 
```
