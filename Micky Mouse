#include<graphics.h>
#include<dos.h>
#include<conio.h>
#include<alloc.h>
void *buf;
void firstleft();
void secondleft();
void main()
{
int gd=DETECT,gm,i=0,x,y,area;
initgraph(&gd,&gm,"tc:\bgi");\put your directory contains egavga.bgi
rectangle(0,0,getmaxx(),getmaxy());
arc(240,120,40,140,70);
ellipse(165,80,10,280,20,20);
ellipse(315,80,-100,170,20,20);
arc(235,120,163,215,70);
arc(245,120,-35,17,70);
ellipse(193,178,85,280,40,20);
ellipse(283,178,-100,95,40,20);
ellipse(238,199,180,0,39,50);
ellipse(213,123,44,240,33,40);
ellipse(262,123,-60,135,33,40);
ellipse(210,123,0,360,13,20);//left eye
ellipse(265,123,0,360,13,20);//right eye
ellipse(210,133,0,360,10,10);//left eye ball
ellipse(265,133,0,360,10,10);//right eye ball
ellipse(210,133,0,360,3,3);//left eye ball
ellipse(265,133,0,360,3,3);//right eye ball
ellipse(238,160,0,360,10,13);//nose
arc(240,125,228,312,68);//mouth
arc(240,120,230,310,72);//mouth
setfillstyle(1,4);
floodfill(238,160,15);//nose
setfillstyle(1,15);
floodfill(210,113,15);
floodfill(265,113,15);
setfillstyle(1,9);
floodfill(210,100,15);
setfillstyle(1,1);
floodfill(315,80,15);
moveto(203,220);
lineto(203,260);
lineto(183,260);
lineto(183,350);
lineto(293,350);
lineto(293,260);
lineto(273,260);
lineto(273,220);
moveto(183,350);
lineto(173,460);
lineto(213,460);
lineto(238,400);
lineto(263,460);
lineto(303,460);
lineto(293,350);
moveto(173,460);
lineto(143,478);
lineto(213,478);
lineto(213,460);
moveto(263,460);
lineto(263,478);
lineto(333,478);
lineto(303,460);
line(238,400,238,350);
//right hand
moveto(183,260);
lineto(113,310);
lineto(183,375);
moveto(183,280);
lineto(137,310);
lineto(181,353);
setfillstyle(2,13);
floodfill(190,300,15);
setfillstyle(1,5);
floodfill(223,400,15);
setfillstyle(1,5);
floodfill(253,400,15);
setfillstyle(1,6);
floodfill(173,470,15);
floodfill(303,470,15);
//fingers
secondleft();
ellipse(413.5,228,0,180,3.5,3.5);
line(420,240,433,240);
line(423,247,440,247);
line(413,240,410,228);
line(417,228,420,240);
ellipse(433,243.5,-90,90,3.5,3.5);
line(423,254,440,254);
ellipse(440,250.5,-90,90,3.5,3.5);
ellipse(430,257,-90,90,3,3);
line(413,260,430,260);
area=imagesize(409,224,444,261);
buf=malloc(area);
getimage(409,224,444,261,buf);
while(!kbhit())
{
if(i==0)
{
setfillstyle(1,15);
setcolor(15);
ellipse(210,133,0,360,10,10);//left eye ball
ellipse(265,133,0,360,10,10);//right eye ball
setcolor(0);
ellipse(210,133,0,360,3,3);//left eye ball
ellipse(265,133,0,360,3,3);//right eye ball
floodfill(210,133,15);
floodfill(265,133,15);
setcolor(0);
putimage(391,209,buf,1);
firstleft();
setcolor(15);
secondleft();
putimage(409,224,buf,0);
i=1;
}
else
{
setfillstyle(1,0);
setcolor(0);
ellipse(210,133,0,360,10,10);//left eye ball
ellipse(265,133,0,360,10,10);//right eye ball
floodfill(210,133,0);
floodfill(265,133,0);
setcolor(15);
ellipse(210,133,0,360,3,3);//left eye ball
ellipse(265,133,0,360,3,3);//right eye ball
floodfill(210,133,15);
floodfill(265,133,15);
setcolor(0);
putimage(409,224,buf,1);
secondleft();
setcolor(15);
firstleft();
putimage(391,209,buf,0);
i=0;
}
delay(300);
}
getch();
}
void firstleft()
{
moveto(293,260);
lineto(353,276);
lineto(395,223);
moveto(293,280);
lineto(355,296);
lineto(395,245);
}
void secondleft()
{
moveto(293,260);
lineto(363,280);
lineto(413,240);
moveto(293,280);
lineto(363,300);
lineto(413,260);
}
