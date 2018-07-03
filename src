
#include<iostream.h>
#include<string.h>
#include<stdio.h>
#include<conio.h>

const N=5;

class cqueue
{
float A[N];
int front;
int rear ;
  public:	
cqueue(){front=-1;rear=-1;}
void addcq();
void delcq();
void dispcq();
};

void cqueue::addcq()					//Addition at the rear
{
if((front==0&rear==N-1)||(front==rear+1))//Checks for Overflow
cout<<"Overflow,addition not possible";
  else
{	rear++;
if (rear==N)rear=0;
cin>>A[rear];
if(front==-1)front=0;
}
}

void cqueue::delcq()					//Deletion at the front
{
if(front==-1||rear==-1)
cout<<"Underflow! queue is empty";	//Checks for Underflow
else
{	if(front==rear)			//Only 1 element present
front=rear=-1;
  else
{	front ++;
if(front==N)front=0;
}
}
}

void cqueue::dispcq()				//Displays the Circular Queue
{
if (rear==-1||front==-1)
cout<<"queue is empty";
  else
{
if(front<=rear)
{	for(int i=front;i<=rear;i++)
cout<<A[i]<<endl;
}
   else
{	for(int k=front;k<N;k++)
cout<<A[k]<<endl;
for(int j=0;j<=rear;j++)
cout<<A[j]<<endl;
}
}
}



void main()
{
int choice;
cqueue cq;
	
do
{
cout<<"1.ADD\n";
cout<<"2.DELETE\n";
cout<<"3.DISPLAY \n";
cout<<"4.QUIT\n";
choice=getch();

switch(choice)
{
case '1': cq.addcq();    break;
case '2': cq.delcq();    break;
case '3': cq.dispcq();    break;
case '4':     break;
default :cout<<"\nWrong Choice Entered !!\n\n";
}
}while(choice!='4');
}

