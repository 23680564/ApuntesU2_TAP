# Apuntes-Unidad-2

## Introduccion 

Los componentes y las librerías son elementos clave en el desarrollo de software actual, ya que permiten organizar las aplicaciones de forma más clara, modular y eficiente. Conforme los sistemas se vuelven más complejos, es necesario dividirlos en partes más pequeñas y manejables, conocidas como componentes, los cuales agrupan funciones específicas y pueden reutilizarse en distintos contextos.

Por su parte, las librerías o paquetes ofrecen un conjunto de herramientas ya desarrolladas que ayudan a resolver problemas comunes, evitando que los programadores tengan que crear todo desde cero. Estas pueden formar parte del propio lenguaje o ser creadas por terceros, ampliando así las posibilidades de desarrollo.

Además, la capacidad de diseñar componentes y librerías propias permite adaptar el software a necesidades particulares, fomentando la reutilización del código, disminuyendo errores y mejorando la organización del sistema. Esta práctica es fundamental para crear aplicaciones escalables y fáciles de mantener, ya que facilita su actualización y evolución.
En este sentido, este documento tiene como propósito estudiar los conceptos, características y usos de los componentes y las librerías, así como resaltar su importancia en el desarrollo de software, brindando una base teórica adecuada para su comprensión y correcta aplicación.

# Componentes y Librerías en Programación

Este repositorio presenta una recopilación teórica sobre los conceptos fundamentales de los componentes y las librerías en el desarrollo de software. Se abordan definiciones, características, tipos, así como su importancia en la construcción de aplicaciones modernas.

El contenido está orientado a comprender cómo estos elementos permiten estructurar, reutilizar y optimizar el código, facilitando el desarrollo de sistemas más eficientes y escalables.

---

## Contenido

- 2.1 Definición conceptual de componentes y paquetes/librerías  
- 2.2 Uso de librerías proporcionadas por el lenguaje  
- 2.3 Creación de componentes definidos por el usuario  
- 2.4 Creación y uso de paquetes/librerías definidas por el usuario  

---

## 2.1 DEFINICIÓN CONCEPTUAL DE COMPONENTES, PAQUETES / LIBRERÍAS

## ¿QUÉ SON LOS COMPONENTES?

En programación, un componente es una pieza de software reutilizable que realiza una función específica y que puede integrarse dentro de programas más grandes sin necesidad de conocer su código interno. Los componentes actúan como "bloques de construcción" que encapsulan funcionalidad y datos, permitiendo que sean usados por otros programas o sistemas a través de interfaces bien definidas. Pueden ser visuales (como botones, ventanas o menús) o no visuales (como conexiones a bases de datos, gestores de archivos o cálculos matemáticos). Su principal ventaja es que facilitan el desarrollo, permiten ahorrar tiempo y hacen que el código sea más organizado y fácil de mantener.
--
## ¿QUÉ SON LAS LIBRERÍAS O BIBLIOTECAS?

Una librería (o biblioteca) es un conjunto de código preescrito, funciones, clases y recursos que ofrecen funcionalidades específicas para ser utilizadas en otros programas. En lugar de escribir todo desde cero, los programadores pueden usar librerías para aprovechar trabajo ya realizado, optimizando el desarrollo y reduciendo errores. Las librerías suelen estar organizadas por temas: manejo de imágenes, conexiones de red, matemáticas, interfaces gráficas, etc.
--
## ¿QUÉ SON LOS PAQUETES?

Un paquete es una forma de organizar y agrupar varias clases, interfaces o librerías relacionadas dentro de una misma estructura, generalmente con el fin de evitar conflictos de nombres y mantener el código ordenado. En muchos lenguajes, los paquetes corresponden a directorios o carpetas en el sistema de archivos donde se almacenan los archivos de código relacionados. Ayudan a modularizar el proyecto y facilitan su gestión y distribución.
--
## DIFERENCIAS Y RELACIONES
- Componente: Es la unidad funcional que se usa directamente.
- Librería: Es el conjunto de componentes o funciones agrupadas.
- Paquete: Es la forma de organizar y agrupar lógicamente las librerías o clases.

Juntos forman el ecosistema que permite el desarrollo modular y reutilizable de software.
--

## 2.2 USO DE LIBRERÍAS PROPORCIONADAS POR EL LENGUAJEz
--
## VENTAJAS
- No requieren instalación externa.
- Están probadas y optimizadas por los creadores del lenguaje.
- Garantizan compatibilidad y estabilidad.
- Cubren necesidades comunes: manejo de archivos, entrada/salida, matemáticas, fechas, cadenas de texto, estructuras de datos, etc.
--
## EJEMPLO DE USO

Por ejemplo, en Python:
- `import math` para funciones matemáticas.
- `import os` para manejo de archivos y carpetas.
- `import datetime` para trabajar con fechas y horas.

En Java:
- `import java.util.ArrayList` para usar listas dinámicas.
- `import java.io.File` para manejo de archivos.

El uso consiste simplemente en importar la librería o clase necesaria al inicio del programa y luego llamar a sus funciones o métodos cuando se requieran.
--

## 2.3 CREACIÓN DE COMPONENTES (VISUALES Y NO VISUALES) DEFINIDOS POR EL USUARIO

## COMPONENTES VISUALES
Son aquellos que tienen representación en la interfaz gráfica y con los que el usuario puede interactuar directamente. Al crear componentes visuales personalizados, se define su apariencia (colores, formas, tamaño) y su comportamiento (qué hacen al hacer clic, al pasar el mouse, etc.).
Ejemplos: botones personalizados, gráficos, tablas, campos de texto con validación, etc.
--
## COMPONENTES NO VISUALES
Son aquellos que no tienen interfaz gráfica pero realizan tareas importantes en segundo plano. Su creación se centra en la lógica y funcionalidad.
Ejemplos: gestores de base de datos, servicios de red, validadores de datos, generadores de reportes, etc.
--
## CÓMO SE CREAN
Generalmente se crean mediante la definición de clases en programación orientada a objetos. Se encapsulan atributos y métodos, y se exponen solo aquellos que deben ser accesibles para otros partes del programa.
- Para visuales: Se heredan de clases base de interfaces gráficas y se sobrescriben métodos de dibujo o eventos.
- Para no visuales: Se crean clases con la lógica necesaria y métodos públicos para interactuar con ellas.
--

## 2.4 CREACIÓN Y USO DE PAQUETES / LIBRERÍAS DEFINIDAS POR EL USUARIO

## CREACIÓN DE PROPIAS LIBRERÍAS
Cuando desarrollamos funciones, clases o componentes que pueden ser útiles en más de un proyecto, podemos agruparlos y organizarlos como una librería propia. Esto permite reutilizar el código fácilmente y compartirlo con otros desarrolladores.
Pasos generales:
1. Escribir el código con las funcionalidades deseadas.
2. Organizarlo en archivos y carpetas de forma lógica.
3. Documentar su uso.
4. Empaquetarlo si es necesario para su distribución.
--
## CREACIÓN DE PAQUETES
En muchos lenguajes, crear un paquete es tan sencillo como crear una carpeta y colocar dentro los archivos de código fuente, agregando al inicio de cada archivo una declaración que indique a qué paquete pertenece.
Ejemplo en Java:
`package mi_paquete.utilidades;`

Ejemplo en Python: Se usa la presencia de un archivo `__init__.py` para indicar que una carpeta es un paquete.
--
## CÓMO SE USAN
Una vez creados, se utilizan igual que las librerías del lenguaje: mediante sentencias de importación.
`import mi_libreria`
`from mi_paquete import mi_clase`
--
## EJEMPLOS DE CÓDIGO VISTOS EN CLASES

### Graficas

<img width="850" height="665" alt="image" src="https://github.com/user-attachments/assets/e59946cf-790e-44c0-9736-97045343ef1b" />

```
import flet as ft
import matplotlib.pyplot as plt
import numpy as np
from io import BytesIO
import base64


# Convertir gráfica a base64
def crear_grafica(fig):
    buffer = BytesIO()
    fig.savefig(buffer, format="png")
    buffer.seek(0)
    img_base64 = base64.b64encode(buffer.read()).decode("utf-8")
    plt.close(fig)
    return img_base64


# Grafica de línea
def grafica_linea():
    x = np.linspace(0, 10, 50)
    y = np.sin(x)

    fig, ax = plt.subplots()
    ax.plot(x, y)
    ax.set_title("Gráfica de Línea")

    return crear_grafica(fig)


# Grafica de barras
def grafica_barras():
    valores = [10, 20, 15, 30]

    fig, ax = plt.subplots()
    ax.bar(["A", "B", "C", "D"], valores)
    ax.set_title("Gráfica de Barras")

    return crear_grafica(fig)


# Grafica de pastel
def grafica_pie():
    datos = [30, 40, 20, 10]

    fig, ax = plt.subplots()
    ax.pie(datos, labels=["A", "B", "C", "D"], autopct="%1.1f%%")
    ax.set_title("Gráfica de Pastel")

    return crear_grafica(fig)


# Grafica de dispersión
def grafica_dispersion():
    x = np.random.rand(50)
    y = np.random.rand(50)

    fig, ax = plt.subplots()
    ax.scatter(x, y)
    ax.set_title("Gráfica de Dispersión")

    return crear_grafica(fig)


def main(page: ft.Page):

    page.title = "Dashboard de Gráficas"
    page.scroll = "auto"

    img1 = ft.Image(src="data:image/png;base64," + grafica_linea())
    img2 = ft.Image(src="data:image/png;base64," + grafica_barras())
    img3 = ft.Image(src="data:image/png;base64," + grafica_pie())
    img4 = ft.Image(src="data:image/png;base64," + grafica_dispersion())

    grid = ft.GridView(
        expand=True,
        runs_count=2,
        max_extent=500,
        child_aspect_ratio=1.0,
        spacing=10,
        run_spacing=10,
        controls=[
            img1,
            img2,
            img3,
            img4,
        ],
    )

    page.add(grid)


ft.app(target=main)
```

### Catalogo
<img width="1365" height="728" alt="image" src="https://github.com/user-attachments/assets/b5f57544-22df-4990-a527-590e0c4e8d02" />

```
import flet as ft

class ProductoCard(ft.Container):
    def __init__(self, nombre, descripcion, precio, imagen_archivo):
        super().__init__()
        self.width = 250
        self.height = 480
        self.bgcolor = "white"
        self.border_radius = 15
        self.padding = 15
        self.shadow = ft.BoxShadow(blur_radius=10, color="grey400")
        
        self.content = ft.Column(
            horizontal_alignment=ft.CrossAxisAlignment.CENTER,
            alignment=ft.MainAxisAlignment.SPACE_EVENLY,
            controls=[
                ft.Image(src=imagen_archivo, width=180, height=120, fit="contain"),
                
                ft.Text(nombre, size=18, weight="bold"),
                ft.Text(descripcion, size=12, color="grey600", text_align="center"),
                ft.Text(f"${precio}", size=20, color="green700", weight="bold"),
                
                ft.Row(
                    alignment=ft.MainAxisAlignment.CENTER,
                    spacing=15,
                    controls=[
                        ft.TextButton(
                            content=ft.Image(src="favorito.png", width=20, height=20),
                            tooltip="Favorito"
                        ),
                        ft.ElevatedButton(
                            content=ft.Row(
                                controls=[
                                    ft.Image(src="carrito.png", width=20, height=20),
                                    ft.Text("Agregar", color="white")
                                ]
                            ),
                            bgcolor="#8ECAE6"  # Azul pastel coordinado
                        )
                    ]
                )
            ]
        )

productos_datos = [
    {"n": "Monitor", "d": "Pantalla 4K Pro", "p": 3500, "i": "monitor.jpg"},
    {"n": "Teclado", "d": "Mecánico RGB", "p": 1200, "i": "teclado.jpg"},
    {"n": "Mouse", "d": "Gamer 16k DPI", "p": 850, "i": "mouse.jpg"},
    {"n": "Audífonos", "d": "Noise Cancelling", "p": 1500, "i": "audifonos.jpg"},
    {"n": "Laptop", "d": "Core i7 16GB RAM", "p": 18000, "i": "laptop.jpg"},
]

def main(page: ft.Page):
    page.title = "Tienda Tech - Catálogo Reutilizable"
    page.bgcolor = "#E0F7FA"  # Azul pastel claro (fondo principal)
    page.scroll = "auto"
    page.horizontal_alignment = ft.CrossAxisAlignment.CENTER

    catalogo = ft.Row(wrap=True, spacing=20, run_spacing=20, alignment=ft.MainAxisAlignment.CENTER)
    for p in productos_datos:
        catalogo.controls.append(ProductoCard(p["n"], p["d"], p["p"], p["i"]))

    page.add(
        ft.Container(
            content=ft.Text("TECH-RECYCLE STORE", size=32, weight="bold", color="#2196F3"),  # Azul más intenso para el título
            padding=30
        ),
        catalogo
    )

if __name__ == "__main__":
    ft.app(target=main, assets_dir="assets")

```

## Componentes con Dataclass
<img width="1264" height="486" alt="image" src="https://github.com/user-attachments/assets/3f912545-a4e6-48b9-96f6-296686a2bb81" />


```
import flet as ft
from dataclasses import dataclass


# Dataclass para almacenar datos
@dataclass
class Usuario:
    nombre: str
    rol: str
    color: str = ft.Colors.BLUE


# Componente visual
class TargetPerfil(ft.Container):

    def __init__(self, usuario: Usuario):
        super().__init__()

        self.usuario = usuario

        self.content = ft.Column(
            controls=[
                ft.Text(usuario.nombre, weight=ft.FontWeight.BOLD, size=20),
                ft.Text(usuario.rol, italic=True),
                ft.ElevatedButton("Ver perfil", on_click=self.saludar)
            ],
            tight=True
        )

        self.border = ft.border.all(2, usuario.color)
        self.padding = 10
        self.border_radius = 10
        self.width = 200

    def saludar(self, e):
        print(f"Interactuando con el componente de {self.usuario.nombre}")


def main(page: ft.Page):

    page.title = "Unidad 2: Componentes con Dataclass"
    page.horizontal_alignment = ft.CrossAxisAlignment.CENTER

    # Crear datos usando dataclass
    usuario1 = Usuario("Ana Garcia", "Desarrolladora Senior", ft.Colors.GREEN)
    usuario2 = Usuario("Carlos Ruiz", "Arquitecto de Software")

    # Crear componentes visuales
    tarjeta1 = TargetPerfil(usuario1)
    tarjeta2 = TargetPerfil(usuario2)

    page.add(
        ft.Text("Lista de Usuarios", size=30, weight="bold"),
        ft.Row(
            [tarjeta1, tarjeta2],
            alignment=ft.MainAxisAlignment.CENTER
        )
    )


ft.app(target=main)
```
### Componentes con Clases
<img width="1245" height="509" alt="image" src="https://github.com/user-attachments/assets/3ea6f58e-e139-4e37-9ec8-b79e4cd9651f" />


```
import flet as ft

# Componente personalizado usando CLASE
class TargetPerfil(ft.Container):

    def __init__(self, nombre, rol, color_borde=ft.Colors.BLUE):
        super().__init__()

        self.nombre = nombre
        self.rol = rol

        self.content = ft.Column(
            controls=[
                ft.Text(nombre, weight=ft.FontWeight.BOLD, size=20),
                ft.Text(rol, italic=True),
                ft.ElevatedButton("Ver perfil", on_click=self.saludar)
            ],
            tight=True
        )

        self.border = ft.border.all(2, color_borde)
        self.padding = 10
        self.border_radius = 10
        self.width = 200

    # Método de la clase
    def saludar(self, e):
        print(f"Interactuando con el componente de {self.nombre}")


def main(page: ft.Page):

    page.title = "Unidad 2: Componentes definidos por el usuario"
    page.horizontal_alignment = ft.CrossAxisAlignment.CENTER

    # Instancias de la clase
    usuario1 = TargetPerfil("Ana Garcia", "Desarrolladora Senior", ft.Colors.GREEN)
    usuario2 = TargetPerfil("Carlos Ruiz", "Arquitecto de Software")

    page.add(
        ft.Text("Lista de Usuarios", size=30, weight="bold"),
        ft.Row(
            [usuario1, usuario2],
            alignment=ft.MainAxisAlignment.CENTER
        )
    )


ft.app(target=main)
```
### Juego de piedra, papel o tijera
<img width="1275" height="550" alt="image" src="https://github.com/user-attachments/assets/ea46a77b-c443-42bc-a52b-0710762b1267" />

```
import flet as ft
import random


def main(page: ft.Page):
    page.title = "Juego: Piedra, Papel o Tijeras"
    page.horizontal_alignment = ft.CrossAxisAlignment.CENTER
    page.vertical_alignment = ft.MainAxisAlignment.START

    # Texto donde se muestra el resultado
    resultado_texto = ft.Text(
        value="Elige una opción para comenzar",
        size=18,
        weight="bold"
    )

    # Función que se ejecuta al presionar un botón
    def jugar(e):
        opciones = ["Piedra", "Papel", "Tijeras"]

        # Obtener lo que eligió el usuario 
        eleccion_usuario = e.control.content.value

        # Elección aleatoria de la máquina
        eleccion_maquina = random.choice(opciones)

        # Determinar ganador
        if eleccion_usuario == eleccion_maquina:
            resultado = " Empate"
        elif (
            (eleccion_usuario == "Piedra" and eleccion_maquina == "Tijeras") or
            (eleccion_usuario == "Papel" and eleccion_maquina == "Piedra") or
            (eleccion_usuario == "Tijeras" and eleccion_maquina == "Papel")
        ):
            resultado = " ¡Ganaste!"
        else:
            resultado = " Gana la máquina"

        # Mostrar resultado
        resultado_texto.value = (
            f"Tú elegiste: {eleccion_usuario}\n"
            f"La máquina eligió: {eleccion_maquina}\n\n"
            f"Resultado: {resultado}"
        )

        page.update()

    # Botones
    botones = ft.Row(
        controls=[
            ft.ElevatedButton(
                content=ft.Text("Piedra"),
                on_click=jugar
            ),
            ft.ElevatedButton(
                content=ft.Text("Papel"),
                on_click=jugar
            ),
            ft.ElevatedButton(
                content=ft.Text("Tijeras"),
                on_click=jugar
            ),
        ],
        alignment=ft.MainAxisAlignment.CENTER
    )

    # Agregar elementos a la página
    page.add(
        ft.Text("Piedra, Papel o Tijeras", size=24, weight="bold"),
        ft.Divider(),
        botones,
        ft.Container(height=20),
        resultado_texto
    )


ft.app(target=main)
```


## BIBLIOGRAFÍA 
- Sommerville, I. (2011). Ingeniería del software. Pearson Educación.
- Deitel, P., & Deitel, H. (2017). Java: Cómo programar. Pearson Educación.
- Van Rossum, G., & Drake, F. L. (2018). The Python Tutorial. Python Software Foundation.
- Gamma, E., Helm, R., Johnson, R., & Vlissides, J. (1995). Design Patterns: Elements of Reusable Object-Oriented Software. Addison-Wesley.
- Pressman, R. S. (2010). Ingeniería del software: Un enfoque práctico. McGraw-Hill.


## Conclusion
En síntesis, los componentes y las librerías son elementos esenciales para desarrollar software eficiente y de buena calidad. Su implementación permite dividir sistemas complejos en partes más simples, lo que facilita su desarrollo, comprensión y mantenimiento. La modularidad que aportan los componentes impulsa la reutilización del código, optimizando el tiempo de trabajo y reduciendo posibles errores.
De igual manera, las librerías, tanto las que vienen integradas en el lenguaje como las creadas por los propios desarrolladores, proporcionan herramientas que simplifican la creación de funcionalidades comunes, permitiendo enfocarse en aspectos más específicos e innovadores de los proyectos. La creación de librerías propias también contribuye a una mejor organización y estructura del código.
En conjunto, el conocimiento y uso adecuado de estos conceptos mejora significativamente la calidad del software y promueve buenas prácticas de programación. Por ello, dominar componentes y librerías es fundamental para cualquier desarrollador que aspire a crear aplicaciones modernas, eficientes y sostenibles a largo plazo.
