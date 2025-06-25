# RETO 5 💀

## Ejercicio 1
- Dado la figura de la imagen, desarrolle:

<div align='center'>
<figure> <img src="https://i.postimg.cc/FRvCmpxx/image.png" alt="" width="400" height="auto"/></br>
<figcaption><b></b></figcaption></figure>
</div>

+ Una función matemática para calcular el volumen y el área superficial.
+ Cree dos funciones en python para calcular los valores antes establecidos, al ingresar por teclado `r1`, `r2` y `h`.
+ Revise como utilizar el valor de `pi` usando *import math* y *math.pi*
```python
import math
#funciones de volumen y area esfera
def volumen_esfera(r1:float) -> float:
    volumen = (4/3)*math.pi*r1**3
    return volumen

def area_esfera(r1:float) -> float:
    area = 4*math.pi*r1**2
    return area
#funciones de volumen y area cono
def volumen_cono(r2:float, h:float) -> float:
    volumen_con = (1/3)*math.pi*r2**2*h
    return volumen_con

def area_cono(r2:float, h:float) -> float:
    area_con = math.pi*r2**2 + math.pi*r2*h
    return area_con

if __name__ == "__main__":
    #datos de entrada usuario
    r1 = float (input("Ingrese el radio de la esfera:"))
    r2 = float (input("Ingrese el radio del cono: "))
    h = float (input("Ingrese la altura del cono: "))
    #volumen y area esfera
    volum_esfera = volumen_esfera(r1)
    are_esfera = area_esfera(r1)
    #volumen y area cono
    volum_cono = volumen_cono(r2, h)
    are_cono = area_cono(r2, h)
    #area y volumen totales
    area_total = are_esfera + are_cono
    volumen_total = volum_esfera + volum_cono
    print(f"Volumen esfera: {volum_esfera:.2f}, Área esfera: {are_esfera:.2f}, Volumen cono: {volum_cono:.2f}, Área cono: {are_cono:.2f}")
    print("Area total: " + str(area_total), "Volumen total: " + str(volumen_total))
```

## Ejercicio 2
- Dado la figura de la imagen, desarrolle:

<div align='center'>
<figure> <img src="https://i.postimg.cc/1t4MrzsL/image.png" alt="" width="400" height="auto"/></br>
<figcaption><b></b></figcaption></figure>
</div>

+ Una función matemática para calcular el área y el perimetro.
+ Cree dos funciones en python para calcular los valores antes establecidos, al ingresar por teclado `r`, `a` y `b`.
+ Revise como utilizar el valor de `pi` usando *import math* y *math.pi*
```python
import math

def area_y_perimetro_rectangulo(b:float, a:float) -> float:
    area = b * a
    perimetro = 2*(b+a)  
    return area, perimetro
def area_y_perimetro_circulo(r:float) -> float:
    area2 = math.pi*r**2
    perimetro2 = 2*r*math.pi
    return area2, perimetro2

if __name__ == "__main__":
    b = float (input("Ingrese la base del rectangulo: "))
    a = float (input("Ingrese la altura del rectangulo: "))
    r = float (input("Ingrese el radio del circulo: "))
    area_rect, perim_rect = area_y_perimetro_rectangulo(b, a)
    area_circ, perim_circ = area_y_perimetro_circulo(r)

    area_total = area_rect + 2 * area_circ
    perimetro_total = perim_rect + 2 * perim_circ

    print("Área y perímetro del rectángulo:", area_rect, perim_rect)
    print("Área y perímetro del círculo:", area_circ, perim_circ)
    print("Área total:", area_total)
    print("Perímetro total:", perimetro_total)
```
# Autor 🤖
- [Juan Carlos Polania Bolivar](https://github.com/Ciyuang)
