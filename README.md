# gi-i-ph-ng-tr-nh-b-c-2
x= input ( " MODE = ")
if x== "1" :
    a,b,c= float( input ( "a : ")),float( input ( "b : ")),float( input ("c : "))
    d= ((b**2)-4*a*c)
    if d < 0 : 
        print ( " vô nghiệm " )
    if d== 0 :
        x = ((-b+(d)**0.5)/(2*a))
        print (x) 
    if d> 0 :
        x1 = ((-b+(d)**0.5)/(2*a))
        x2 = ((-b-(d)**0.5)/(2*a))
        print (x1)
        print (x2) 
