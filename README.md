# ellipse-algorithm
rx=int(input("Enter major axis:"))
ry=int(input("Enter minor axis:"))
xc=int(input("Enter center x:"))
yc=int(input("Enter center y:"))
x=0
y=ry
P0=(ry**2)-(rx**2)*ry+0.25*(ry**2)
k=0
while((2*(ry**2)*x)<(2*(rx**2)*y)):
    if(P0<0):
        x=x+1
        P0=P0+2*(ry**2)*x + (ry**2) 
    else:
        x=x+1
        y=y-1
        P0=P0+2*(ry**2)*x - 2*(rx**2)*y + (ry**2)
    print (x,y)
    k=k+1

P20=((ry**2)*(x+0.5)**2)+((rx**2)*(y-1)**2)-(rx**2)*(ry**2)
k=0
while(y!=0):
    if(P20>0):
        y=y-1
        P20=P20-2*(rx**2)*y+(rx**2)
    else:
        x=x+1
        y=y-1
        P20=P20-2*(rx**2)*y + 2*(ry**2)*x + (rx**2)
    print(x,y)
    k=k+1
