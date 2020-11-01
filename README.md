# array-list-implement
#include<stdio.h>
#include<conio.h>
#define max=10
void create();
void insert();
void deletion();
void search();
void display();
int a, b[20],n,p,e,f,i,pos;
void main()
{
clrscr();
int ch;
char g='y';
do{
printf("\n main menu");
printf("\n1.create \n2.delete \n3.search \n4.insert \n5.display \n6.exit\n");
printf("\n enter your choice");
scanf("%d",&ch);
switch(ch)
{
case 1:
create();
break;
case 2:
deletion();
break;
case 3:
search();
break;
case 4:
insert();
break;
case 5:
display();
break:
case 6:
exit();
break;
default:
printf("\n enter the correct choice:");
}
printf("\n do you want to continue?");
scanf("\n%c",&g);
}
while(g=='y'||g=='Y');
getch();
}
void create()
{
printf("\n enter the number of nodes");
scanf("%d",&n);
for(i=0;i<n;i++)
{
 printf("\n enter the element:",i+1);
 scanf("%d",&b[i]);
 }
 }
 void deletion()
 {
 printf("\n enter the position you want to delete:");
 scanf("%d",&pos);
 if(pos>=n)
 {
  printf("\n invalid location");
  }
  else
  {
  for(i=pos+1;i<n;i++)
  {
   b[i-1]=b[i];
   }
   n--;
   }
   printf("\n elements after the deletion:");
   for(i=0;i<n;i++)
   {
    printf("\t%d",b[i]);
    }
    }
    void search()
    {
     printf("\n enter the element to be searched:");
     scanf("%d",&e);
     for(i=0;i<n;i++)
     {
       if9b[i]==0)
       {
        printf("value is in the %d position",i);
        }}}
        void insert()
        {
         printf("\n enter the position u need to insert:");
         scanf("%d",&pos);
         if(pos>=n)
         {
          printf("\n invalid location");
          }else
          {
           for(i=max-1;i>=pos-1;i--)
           {
            b[i+1]=b[i];
            }
            printf("\n enter the element to insert:\m");
            scanf("%d",&p);
            b[pos]=p;
            n++;
            }
            printf("\n the list after the insertion:\n");
            display();
            }
            void display(){
            printf("\n the elements of the list adt are:");
            for(i=0;i<n;i++)
            {
            printf("\n\n%d",b[i]);
            }}
