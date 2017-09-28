# 源代码
'
import math

v=0; #velocity at first is "0"#

t=0; #time#

a,b=10,1; #two external parameter#

 #a means gravity;b means friction factor#
 
ts=0.01 #time step#

while t<=5:

    import pylab as pl
    
    pl.scatter(t,v)
    
    pl.title('Plot of v vs. t')
    
    pl.xlabel('t /s')
    
    pl.ylabel('v / m/s')
    
    v=v+a*math.exp(-b*t)*ts #taylor expansion with Euler's method#
    
    t=t+ts'
