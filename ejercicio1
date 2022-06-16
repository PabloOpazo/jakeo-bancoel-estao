import time


print('jakeo bancoel estao')

def iva(presio):
    iva = presio * 1.19
    return(iva)

def descuento(presio,dcto):
    descuento = presio - (presio*dcto/100)
    return(round(descuento))

def imc(peso,altura):
    imc = float(peso / pow((altura/100),2))
    imc = round(imc,1)
    #print(imc)
    if imc<18.5:
        estado = 'BAJO PESO'
        
    elif imc>=18.5 and imc<=24.9:
        estado = 'ADECUADO'
    
    elif imc>=25 and imc<=29.9:
        estado = 'SOBREPESO'
    
    elif imc>=30 and imc<=34.9:
        estado = 'OBESIDAD 1'
    
    elif imc>=35 and imc<=39.9:
        estado = 'OBESIDAD 2'
    
    elif imc>=40:
        estado = 'OBESIDAD 3'
    
    #print(estado)
    return('IMC: ' + str(imc) + '\nEstado:'+ estado)

def volver_menu_principal():
    time.sleep(5)
    print('volviendo al menú principal...')
    time.sleep(2)

while True:
    try:
        print('MENÚ:\n 1. Calcular el IVA\n 2. Calcular Descuento\n 3. Calcular IMC\nPara finalizar escriba "salir"\n\n')
        menu = input('Ingrese el numero de la opción deseada: ')
        
        if menu=='1':
            print('\nCalcular el IVA\n')
            
            precio = int(input('Ingrese el precio del producto sin IVA: '))
            
            print(f"El Valor del producto + IVA = ${int(iva(precio))}")
            volver_menu_principal()
             
        elif menu=='2':
            print('\nCalcular Descuento\n')
            precio = int(input('Ingrese el precio del producto: '))
            dscto = int(input('ingrese el porcentaje de descuento (por ej. 20): '))

            print(f'precio del producto: ${precio} \nDescuento: {dscto}% \nprecio final: ${descuento(precio,dscto)}')
            volver_menu_principal()
            
        elif menu=='3':
            print('\nCalcular IMC\n')
            
            peso = int(input('Ingrese el peso (Kg): '))
            altura = float(input('Ingrese altura (cm): '))
            
            print(imc(peso,altura))
            volver_menu_principal()
        
        elif menu=='salir':
            print('\n gracias por jakear al bancoel estao 🤑😈💸\n\n\n\n')
            break    
    except:
        print("opción inválida")
