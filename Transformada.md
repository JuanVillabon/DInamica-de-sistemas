# Transformada de LaPlace
## 1. Que es la transformada de laPlace
El método de la transformada de Laplace es una herramienta operacional útil para resolver ecuaciones diferenciales lineales con coeficientes constantes. Utilizada para convertir funciones del dominio del tiempo en funciones del dominio de la frecuencia. Es especialmente útil en el análisis y diseño de sistemas lineales, así como en la resolución de ecuaciones diferenciales. Esto permite que la solución de la ecuación diferencial se obtenga mediante tablas de transformadas de Laplace o utilizando la técnica de fracciones parciales.
## 2. Que es la transformada inversa de LaPlace
La transformada inversa de Laplace es el proceso de recuperar la función original del dominio del tiempo a partir de su representación en el dominio de la frecuencia obtenida mediante la transformada de Laplace. Si las funciones son simples utilizar la tabla de transformadas, pero si las funciones son una combinación o una composición de varias funciones; calcular la integral de la definición de la transformada inversa de LaPlace.
## 3. Definiciones
### 3.1. Transformada de LaPlace
f(t) = Una funcion del tiempo

s = Una variable compleja

L = Transformada por la integral de Laplace

F(s) = transformada de Laplace de f(t)

$$ L[f(t)] = F(s) $$

$$ \lim_{0 \to \infty} e^{-st} dt[f(t)] = \lim_{0 \to \infty} f(t)e^{-st} $$

### 3.2. Transformada inversa de LaPlace
La notación de la transformada inversa de Laplace es $L^{-1}$

$$ L^{-1} [F(s)] = f(t) $$

## 4. Propiedades de la transformada de LaPlace
### 4.1. Linealidad:
$$ L[C_{1}f(t) + C_{2}g(t)] = C_{1}L[f(t)] + C_{2}L[g(t)] $$ 

$$ C_{1} , C_{2} \mathbb{E} \mathbb{R} $$
### 4.2. Desplazamineto en t
Si $g(t) = f(t - T) \mathbb{u} (t - T)$

Entonces $G(s) = e^{-st} F(s) , T \geq 0$
### 4.3. Desplazamiento en s

si $g(t) = e^{-at} f(t)$

entonces $G(s) = F(s + a) , a \geq 0$
### 4.4. Escalado en t
si $g(t) = f(kt)$

entonces $G(s) = \frac{1}{k} * F * (\frac{s}{k})$

## 5. Tipos de Transformadas
### 5.1. Transformada escalon unitario
Definicion de la funcion escalon: 

$f(t) = 0$ para $t < 0$

$f(t) = A$ para $t > 0$

Donde A es una constante, 

💡**Ejemplo:**

$1(t) = 0$ para t < 0

$1(t) = 1$ para t > 0

$$ L[1(t)] = \frac{1}{s} $$

### 5.2. Transformada función rampa

$f(t) = 0$ para t < 0

$f(t) = At$ para t \geq 0

💡**Ejemplo:**

$$ L[At] = \lim_{0 \to \infty} Ate^{-st} dt = At \frac{e^{-st}}{-s} - \lim_{0 \to \infty} \frac{Ae^{-st}}{-s} dt $$

$$ \frac{A}{s} \lim_{0 \to \infty} e^{-st} dt = \frac{A}{s^{2}} $$

### 5.3. Transformada función senosoidal

$f(t) = 0$  para t < 0

$f(t) = A sen wt$ para t \geq 0

💡**Ejemplo:**

$$ sen wt = \frac{1}{2j}(e^{jwt} - e^{-jwt}) $$

$$ L[A sen wt] = \frac{A}{2j} \lim_{0 \to \infty} (e^{jwt} - e^{-jwt}) e^{-st} dt $$

$$ = \frac{A}{2j} \frac{1}{s-jw} - \frac{A}{2j} \frac{1}{s+jw} = \frac{Aw}{s^{2}+w^{2}} $$

## 6. Transformadas
### 6.1. Transformada de una función
$$ L[f(t) = F(s) $$
### 6.2. Transformada de la derivada
$$ L[f'(t)] = sF(s) - f(0) $$

$$ L[f''(t) = s^{2}F(s) - sf(0) - f'(0) $$

$$ L[f^{n}] = s^{n}F(s) - s^{n-1}f(0) - - - - sf^{n-1}(0) - f^{n}(0) $$

### 6.3. Transformada de la integral
$$ L(\lim_{\to \} f(t) dt ) = \frac{1}{s} * F(s) $$

## 7. Tabla de transformadas

![tabla-transformada-laplace-a](https://github.com/user-attachments/assets/125c240a-e3b5-4ecb-ac40-3c8dc9a7dcd7)

## 8. 📚 Ejercicios

📚 Halle la transformacion de la siguiente funcion: $L[t^{3}+5t^{2}-3t+8]$

$$ L[t^{3}] + 5L[t^{2}] - 3L[t^{2}] + L[8]

$$ = \frac{3!}{s^{4}} + 5\frac{2!}{s^{3}} - 3\frac{1!}{s^{2}} + \frac{8}{s} $$

$$ = \frac{6}{s^{4}} + \frac{10}{s^{3}} - \frac{3}{s^{2}} + \frac{8}{s} $$

📚 Halle la transformada inversa de la siguiente funcion: $L^{-1} [\frac{1}{s^{2}+s-2}$

$$ = \frac{1}{(s+2)(s-1)} = \frac{A}{s+2} + \frac{B}{s-1} $$

$$ 1 = A(s-1) + B(s+2) $$

si s=1 $B = \frac{1}{3}$

si s=-2 $A = \frac{-1}{3}$

$$ \frac{-1}{3} L^{-1} [\frac{1}{s+2} + \frac{1}{3} L^{-1} [\frac{1}{s-1} $$

$$ = \frac{-1}{3} e^{-2t} + \frac{1}{3} e^{t} $$



