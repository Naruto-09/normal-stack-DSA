# normal-stack-DSA
To represent array elements as a stack characteristics 
#include"stdio.h"
#include"stdlib.h"
int top=-1;
int a[5];
int s,i;
void box()
{
     //to print the stack as per logical reprsentation//
     printf("|%d|\n",a[i]);
     printf("~~~\n");
           
 }
void push()
{
      //to enter an element in stack//
      if(top==4)
      {
            printf("\n over-flow : \n");
      }
      else
      {
            printf("\nEnter element in the stack :\n");
            scanf("%d",&s);
            a[top+1]=s;
            top++;
            printf("element is inserted : [%d] \n",a[top]);
      }
}
void pop()
{
      //to remove element in stack//
      if(top==4)
      {
            printf("overflow\n");
      }
      else
      {
            s=a[top];
            top--;
            printf("Element is removed : %d \n",s);
      }
}
void peak()
{
          //to top element in stack//
          if(top==-1)
          {
                printf("Stack is empty : ");
          }
          else
          {
             printf("[%d]",s=a[top]);
          }
            
 }
void display()
{
      //to display an arranged stack//
      if(top==-1)
      {
           printf("Stack is empty : ");
      }
      else
      {
            printf("Stack contains : \n");
            for(i=top ; i>=0 ; i--)
            {
                  
                  box();
             }
      }
            
}      
int main()
{
      int ch;
      do
      {
            printf("\n1- insert\n");
            printf("2- remove\n");
            printf("3- top ele\n");
            printf("4- Display\n");
            printf("5-exit\n");
            printf("Enter your choice=");
            scanf("%d",&ch);
            printf("~~~~~~~~~~~~~~~\n");
            
            switch(ch)
            {
                  case 1 :
                      push();
                      break;
                  case 2:
                      pop();
                      break;
                  case 3:
                      peak();
                      break;
                   case 4:
                       display();
                       break;
                   case 5:
                        exit(0);
                      
            }
      }while(1);
            
}
