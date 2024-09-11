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

### 3.2. Transformada inverda de LaPlace
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
### 5.2. Transformada función rampa
### 5.3. Transformada función senosoidal
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


## 8. Ejercicios




