# SI-LA-VEO
#VAMOS A PASAR . ICC

def  DecimalAHexadecimal (): 
    decimal =  int ( entrada ( " Ingrese un número positivo para convertirlo a hexadecimal: " )) 
    hexadecimal =  " "  
    mientras decimal ! =  0 :
        rem = CambiarDigitos (decimal %  16 )
        hexadecimal =  str (rem) + hexadecimal
        decimal =  int (decimal /  16 )
    print ( " Resultado: "  + hexadecimal)

def  CambiarDigitos ( digitos ): 
    decimales =      [ 10 , 11 , 12 , 13 , 14 , 15 ]
    hexadecimal = [ " A " , " B " , " C " , " D " , " E " , " F " ]
    para c en el  rango ( 7 ):
        si digitos == decimales [c -  1 ]:
            digitos = hexadecimal [c -  1 ]
    regresar digitos

DecimalAHexadecimal ()
