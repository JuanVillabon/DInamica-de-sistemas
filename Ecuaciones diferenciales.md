# Dinamica de Sistemas

## 1. Contenido

### 1.1. Temas:

a. Definiciones

b. Solucion de ecuaciones diferenciales

c. Modelamiento de sistemas : Sistemas mecanicos, Sistemas Electricos, Sistemas Hidraulicos, Sistemas Termicos

d. Funciones de transferencia

e. Diagramas de bloque

f. Algebra de bloques

g. Diagrama de flechas

h. Analisis de sistemas 1 y 2 orden

### 1.2. Software:
a. Matlab
b. Simulador de circuitos

### 1.3. Evaluaciones
| **Criterio**   | **Porcentajes** |
|--------------- |-----------------|
| Autoevaluacion |       10%       |
| Coevaluacion   |       10%       |
| Parcial        |       40%       |
| Tareas         |       30%       |
| Apuntes        |       10%       |

### 1.3. Bibliografias:
- Dinamica de sistemas; Ogata
- Ingenieria de control moderna; Ogata
- Control automatico de procesos; Smith y Corripio

## 2. Definiciones

### 2.1. Sistema:
Un sistema es una combinacion de componentes que actuan conjuntamente para alcanzar un objetivo especifico. La combinacion de componentes se puede representar por medio de reglas o principios que relacionan salidas con las entradas

### 2.2. Sistema dinámico:
es un concepto matemático que describe cómo cambia un sistema con el tiempo. Estos sistemas se modelan utilizando ecuaciones diferenciales,  y pueden ser aplicados en una amplia gama de disciplinas como la física, biología, economía, e ingeniería.

### 2.3. Planta:
el término planta se refiere al sistema físico o proceso que se desea controlar o analizar. Es el objeto o sistema sobre el cual se actúa mediante un controlador, y su comportamiento se describe a través de ecuaciones matemáticas

### 2.4. Proceso:
el término proceso se refiere al conjunto de acciones, interacciones o transformaciones que ocurren dentro de un sistema y que influyen en su comportamiento a lo largo del tiempo.

### 2.5. Modelos dinamicos
es una representación matemática o conceptual que describe cómo un sistema cambia con el tiempo. Los modelos dinámicos se utilizan para predecir el comportamiento de sistemas complejos en función de sus entradas, estados internos y reglas de evolución.

## 3. Ecuaciones diferenciales
### 3.1. Sistemas lineales y no lineales
- Un sistema se condera lineal cuando cumple con el principio de superposicion
- Un sistema lineal tambien tiene la caracteristica de proporcionalidad entre la entrada y la salida
- Los sistemas no lineales no cumplen con el principio de superposicion
- Los sistemas no lineales se linealizan en un punto de operacion, en el cual se cumple el principio de superposicion

### 3.2. Carateristicas:

- Ecuacion lineal invariante en el tiempo

$$ \frac{d^{2}c(t)}{dt^{2}} + 5 \frac{dx(t)}{dt} + 10x(t) = 0 $$

- Ecuacion lineal variane en el tiempo

$$ \frac{d^{2}c(t)}{dt^{2}} + (1 - cos(2t))x(t) = 0 $$

- Ecuacion no lineal variante en el tiempo

$$ \frac{d^{2}c(t)}{dt^{2}} + (x^{2}(t) - 1) \frac{dx(t)}{dt} + x(t) = 0 $$

- Ecuacion no lineal invariante en el tiempo

$$ \frac{d^{2}c(t)}{dt^{2}} + \frac{dx(t)}{dt} + x(t) + x^{t}+ x^{3}(t) = sen (wt) $$

## 3.3. Metodologia de solución

Aplicar transformada de LaPlace a toda la ecuación (término a término), de tal manera que se obtenga una ecuacion algebraica en el dominio de s
Despejar la variable que representa la salida de la ecuación.
Aplicar transformada inversa de LaPlace a la expression obtenida para obtener la solución en el dominio del tiempo.

💡**Ejemplo**
Aplicando transformada inversa desde las tablas para volver al dominio del tiempo

$$ x(t) = L^{-1}[X(s)] = L^{-1} [\frac{2a+b}{s+1} - L^{-1} [\frac{a+b}{s+2}] $$

$$ = (2a + b)e^{-t} - (a + b)e^{-2t}  (t \geq 0) $$

