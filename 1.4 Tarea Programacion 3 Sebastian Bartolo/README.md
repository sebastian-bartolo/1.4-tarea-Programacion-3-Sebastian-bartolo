# 1.4 Tarea Programacion 3 Sebastian Bartolo

### Direcciones

Mostrare lo mi tarea el como lo elabore por puntos con ejemplos de código y diagramas que hice en MERMAID.

---

#### **1. Descripción de los tipos de datos primitivos en C#**

En C#, los tipos de datos primitivos se dividen en tipos por valor y tipos por referencia.

**Tipos por valor:**
- **Enteros (int, short, long, byte):** Me parece ideal para almacenar números enteros. Por ejemplo, un contador de elementos:

```csharp
int contador = 10;
```

- **Flotantes (float, double, decimal):** Se pueden utilizan para valores de punto flotante, como precios:

```csharp
decimal precio = 19.99m;
```

- **Booleanos (bool):** Representan verdadero o falso, como para validar una condición:

```csharp
bool esActivo = true;
```

- **Carácteres (char):** Se puede almacenan un solo carácter, como una inicial:

```csharp
char inicial = 'A';
```

**Tipos por referencia:**
- **String:** Para cadenas de texto, como un nombre:

```csharp
string nombre = "Juan";
```

- **Objetos (object):** Se puede almacenar cualquier tipo de dato, como un valor genérico:

```csharp
object dato = 42;
```

Ejemplo: Para almacenar y manejar datos de un usuario, como nombre, edad y estado activo, usaría `string`, `int` y `bool` respectivamente.

---

#### **2. Comparación de los operadores entre Java y C#**

Pude ver que ambos lenguajes comparten muchos operadores similares, pero hay grandes diferencias que pude ver:

1. **Operadores aritméticos:** `+`, `-`, `*`, `/`, `%` funcionan igual en ambos lenguajes.
2. **Operadores de asignación:** Java y C# usan `=`, `+=`, `-=`, etc., de la misma manera.
3. **Operadores lógicos:**
    - Java: `&&`, `||`, `!`
    - C#: Idénticos, pero también admite el operador `&` y `|` como alternativas para lógica bit a bit o lógica pura.

**Ejemplo en Java:**
```java
int a = 5, b = 10;
boolean resultado = (a < b) && (b > 5);
```

**Ejemplo en C#:**
```csharp
int a = 5, b = 10;
bool resultado = (a < b) && (b > 5);
```

4. **Operadores de igualdad:**
    - Java: Usa `==` para comparar valores primitivos y `equals()` para objetos.
    - C#: Usa `==` tanto para primitivos como para objetos (sobrecargable).

**Ejemplo en C#:**
```csharp
string texto1 = "Hola";
string texto2 = "Hola";
bool sonIguales = texto1 == texto2; // True
```

---

#### **3. Relación entre Solution, Project, Namespace y Clase en C#**

En C#, estos conceptos están jerárquicamente relacionados:

1. **Solution:** Representa el contenedor principal, que puede tener múltiples proyectos.
2. **Project:** Cada proyecto tiene su propio código, bibliotecas y configuraciones.
3. **Namespace:** Agrupa clases y otros elementos dentro de un proyecto.
4. **Clase:** Define el comportamiento y estructura de objetos.

**Ejemplo en código:**
```csharp
// Namespace
namespace MiAplicacion {
    // Clase
    public class Programa {
        public static void Main(string[] args) {
            System.Console.WriteLine("Hola, mundo!");
        }
    }
}
```
---

#### **4. Comparación del control de flujo y operadores condicionales entre Java y C#**

Java y C# tienen estructuras de control similares, pero con algunas diferencias sutiles:

1. **If-else:**
    - Idéntico en ambos lenguajes.

**Ejemplo en Java:**
```java
if (x > 0) {
    System.out.println("Positivo");
} else {
    System.out.println("No positivo");
}
```

**Ejemplo en C#:**
```csharp
if (x > 0) {
    Console.WriteLine("Positivo");
} else {
    Console.WriteLine("No positivo");
}
```

2. **Switch:**
    - En Java, admite Strings desde Java 7. En C#, siempre lo ha soportado.
    - C# permite `when` en casos.

**Ejemplo en C#:**
```csharp
switch (opcion) {
    case 1:
        Console.WriteLine("Uno");
        break;
    case 2 when (esActivo):
        Console.WriteLine("Dos activo");
        break;
    default:
        Console.WriteLine("Otro");
        break;
}
```

3. **Ternario:** Igual en ambos lenguajes:
```java
resultado = (x > 0) ? "Positivo" : "Negativo";
```
```csharp
resultado = (x > 0) ? "Positivo" : "Negativo";
```
---

#### **Diagrama MERMAID**

![Captura de pantalla 2025-01-18 213904.png](img/Captura%20de%20pantalla%202025-01-18%20213904.png)

---

![Captura de pantalla 2025-01-18 214505.png](img/Captura%20de%20pantalla%202025-01-18%20214505.png)

---

![Captura de pantalla 2025-01-18 214539.png](img/Captura%20de%20pantalla%202025-01-18%20214539.png)