#include<graphics.h> 
#include<conio.h> 
#include<alloc.h> 
#include<dos.h> 
#include<stdlib.h> 
void *ball;
void image() 
{ 
//ball 
setcolor(RED); 
setfillstyle(SOLID_FILL,RED); 
fillellipse(10,10,10,10); 
ball=malloc(imagesize(0,0,20,20)); 
getimage(0,0,20,20,ball); 
cleardevice();
}
void main() 
{ 
int gm,gd=DETECT; 
initgraph(&gd,&gm,""); 
int l=getmaxx()/2,r=0,t=0,b=0; 
int x=1,y=1; 
int s=0,key=0; 
int xstep=1,ystep=1;
image(); 
setbkcolor(GREEN);
while(key!=27) 
{
while(!kbhit()){ 
putimage(l,t,ball,XOR_PUT); 
delay(5); 
putimage(l,t,ball,XOR_PUT);
if(l>=getmaxx()||l<=0){x*=-1;sound(1000);s=0;xstep=x*(random(4)+1);ystep=y 
*(random(3)+1);if(l<=0)l=0;else l=getmaxx();}
if(t>=getmaxy()||t<=0){y*=-1;sound(1000);s=0;ystep=y*(random(4)+1);xstep=x 
*(random(3)+1);if(t<=0)t=0;else t=getmaxy();} 
l+=x+xstep; 
t+=y+ystep; 
s++; 
if(s==5) 
{nosound();} 
} 
key=getch();
} 
closegraph(); 
}
