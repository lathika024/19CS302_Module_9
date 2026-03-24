# EX 43 C program to Write a function to display queue elements using array.
## DATE:
## AIM:
To Write a function to display queue elements using array.

## Algorithm
1.Start the program and declare a stack array and a variable top initialized to -1.

2.Define push() to insert an element into the stack if it is not full.

3.Define pop() to remove the top element from the stack if it is not empty.

4.Define peek() to return the topmost element without removing it.

5.Define display() to print all stack elements from top to bottom.
## Program:
```
/*

*/
#include <stdio.h>
#define MAX 100

int queue[MAX];
int front = -1, rear = -1;

void display()
{
    if(front == -1 || front > rear)
    {
        printf("Queue is empty\n");
        return;
    }

    printf("Queue elements: ");
    for(int i = front; i <= rear; i++)
    {
        printf("%d ", queue[i]);
    }
    printf("\n");
}

int main()
{
    front = 0;
    rear = 3;
    queue[0] = 10;
    queue[1] = 20;
    queue[2] = 30;
    queue[3] = 40;

    display();

    return 0;
}


```

## Output:

<img width="424" height="228" alt="442494432-f6288feb-99c7-4907-8724-1af90badf755" src="https://github.com/user-attachments/assets/8113c2ff-2074-4f4e-8445-9803b1b7a7cf" />


## Result:
Thus the program was executed and the output was verified successfully.
