# gi-i-ph-ng-tr-nh-b-c-2
while loop: 
    x= input ( " MODE = ")
    if x== "1" :
        # Phương trình bậc 2 
        a,b,c= float( input ( "a : ")),float( input ( "b : ")),float( input ("c : "))
        d= ((b**2)-4*a*c)
        if d < 0 : 
            print ( " vô nghiệm " )
        if d== 0 :
            x = ((-b+(d)**0.5)/(2*a))
            print ("x=",x) 
        if d> 0 :
            x1 = ((-b+(d)**0.5)/(2*a))
            x2 = ((-b-(d)**0.5)/(2*a))
            print ("x1=",x1)
            print ("x2=",x2) 
    elif x== "2" :
        #khổ dâm hình không gian
        print ( " A ") 
        xA,yA,zA= float( input ( "xA : ")),float( input ( "yA : ")),float(input("zA : "))
        print ( " B ") 
        xB,yB,zB= float( input ( "xB : ")),float( input ( "yB : ")),float(input("zB : "))
        print ( " C ") 
        xC,yC,zC= float( input ( "xC : ")),float( input ( "yC : ")),float(input("zC : "))
        print ( " D ") 
        xD,yD,zD= float( input ( "xD : ")),float( input ( "yD : ")),float(input("zD : "))
        xAB,yAB,zAB,xAC,yAC,zAC,xAD,yAD,zAD= (xB-xA),(yB-yA),(zB-zA),(xC-xA),(yC-yA),(zC-zA),(xD-xA),(yD-yA),(zD-zA)
        x1 = (yAB*zAC-yAC*zAB)*xAD
        x2 = (zAB*xAC-xAB*zAC)*yAD
        x3 = (xAB*yAC-xAC*yAB)*zAD
        VABCD= (1/6)*abs(x1+x2+x3)
        print ("VABCD=",VABCD)
    elif x== "3" :
        # 2 phuong trinh 2 an 
        a1,b1,c1= float( input ( "a1 : ")),float( input ( "b1 : ")),float(input("c1 : "))
        a2,b2,c2= float( input ( "a2 : ")),float( input ( "b2 : ")),float(input("c2 : "))
        x = ((c1*b2-c2*b1)/(a1*b2-b1*a2))
        y = ((c1*a2-a1*c2)/(b1*a2-a1*b2))
        print ("x=",x)
        print ("y=",y)
    elif x== "off" :
        loop = False
