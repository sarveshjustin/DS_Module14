# Ex no:2(E) Applications of Queue – FCFS
## DATE:3/3/25
## AIM:
To write a C function to calculate the turnaround time of each process given their burst time and waiting time in First Come first Serve scheduling algorithm.
## Algorithm
1. Start
2. Define a queue with a fixed size SIZE and initialize front and rear pointers.
3. Define the deQueue() function to remove and return an element from the front of the queue.
4. Check if the queue is empty using isEmpty(); if empty, print an error message.
5. If the queue has one element, reset both front and rear to -1.
6. If the queue has more than one element, update front to the next index using modulo 
operation ((front + 1) % SIZE).
7. Return the removed element from the front of the queue.
8. End
## Program:
```
/*
Program to find and display the priority of the operator in the given Postfix expression
Developed by: sarvesh s
RegisterNumber: 212222230135 
*/
```
```
#include<stdio.h> 
#define SIZE 5
int items[SIZE];
int front =-1,rear =-1;
int deQueue()
{
int element; 
element=items[front]; 
if(isEmpty())
{
printf("Queue isEmpty!!");
}
else
{
if(front==rear)
{
front=-1; 
rear=-1;
}
else
{
front=(front+1)%SIZE;
}
}
return element;
}
```

## Output:

![image](https://github.com/user-attachments/assets/a4005052-7622-4f0a-ba23-8223cbaf331e)




## Result:
Thus, the C function to calculate the turnaround time of each process given their burst time and waiting time in First Come first Serve scheduling algorithm is implemented successfully.
