# Descomposicion en fracciones parciales
## 1. Caso 1. $Q(s)$ tiene raíces reales distintos:

$$ G(s) = \frac{P(s)}{Q(s)} = \frac{P(S)}{(s+p_{1})(s+p_{2})----(s+p_{n})} $$

La descomposición en fracciones parciales es de la forma:

$$ G(s) = \frac{A}{(s+p_{1})} + \frac{B}{(s+p_{2})} + ---- + \frac{N}{(s+p_{n})} $$

Donde A, B, ...... , N coeficientes por determinar.

### 1.1. Ejercicio: $\frac{3x-1}{(x+3)(x-2)}$

$$ \frac{A}{x+3} + \frac{B}{x-2} $$

$$ 3x - = A(x-2) + B(x+3) $$

$$ 3x -1 = Ax -2A + Bx + 3B $$

$$ 3 = A + B $$

$$ A = 3 - B $$

$$ -1 = -2A + 3B $$

$$ -1 = -2(3 - B) + 3B $$

$$ -1 = -6 + 2B + 3B $$

$$ 6 - 1 = 5B $$

$$ 5 = 5B $$

$$ \frac{5}{5} = B $$ 

$$ 1 = B $$

$$ 3 = A + B $$

$$ 3 = A + 1 $$

$$ 3 - 1 = A $$

$$ 2 = A $$

### 1.2 Método resumido (Caso 1)

$$ F(s) = \frac{A(s)}{B(s)} = \frac{a_{1}}{s+p_{1}} + \frac{a_{2}}{s+p_{2}} + ...... + \frac{a_{n}}{s+p_{n}} $$

Sabiendo que $a_{k} (k=1,2,3,...)$ son constantes, $a_{k}$ puede hallarse multipicando ambos lados de la igualdad por $(s+p_{k})$ y haciendo $s = -p_{k}$, de lo cual se obtiene

$$[(s+p_{k}\frac{A(s)}{B(s)}]_{s=-pk} = $$

$$ [\frac{a_{1}}{(s+p_{1}}(s+p_{k}) + \frac{a_{2}}{s+p_{2}}(s+p_{k}) + .... + \frac{a_{k}}{s+p_{k}}(s+p_{k}) + .... + \frac{a_{n}}{s+p_{n}}(s+p_{k})]_{s=-pk} $$

Se cancelan todas menos $a_{k}$

$$ a_{k} = [(s+p_{k}) \frac{S(s)}{B(s)}]_{ s = -pk} $$


## 2. Caso 2. $Q(s)$ tiene n raíces reales repetidos:

$$ G(s) = \frac{P(s)}{Q(s)} = \frac{P(S)}{(s+p)^{n}} $$

La descomposición en fracciones parciales es de la forma:

$$ G(s) = \frac{A}{(s+p)} + \frac{B}{(s+p)^2} + .... + \frac{N}{(s+p)^n} $$

Donde A, B, ...... , N coeficientes por determinar.

### 2.1. Ejercicios:

$$ \frac{7x^{2}+2x-28}{(x-6)(x^{2}+3x+5)} = \frac{A}{x-6} + \frac{Bx+C}{x^{2}+3x+5} $$

$$ 7x^{2} + 2x - 28 = A(x^{2} + 3x + 5) + (Bx + C)(x - 6) $$

$$ 7(6)^{2} + 2(6) - 28 = A((6)^{2} + 3(6) + 5) +(B(6) + C)(6 - 6) $$

$$ 236 = 59A $$

$$ A = 4 $$

$$ 7 = A + B $$

$$ 7 = 4 + B $$

$$ 7 - 4 = B $$

$$ 3 = B $$

$$ -28 = 5A - 6C $$

$$ -28 = 5(4) - 6C $$

$$ -28 = 20 - 6C $$

$$ -28 - 20 = - 6C $$

$$ \frac{-48}{-6} = C $$

$$ 8 = C $$

### 2.2. Metodo resumido Caso 2.
Se puede aplicar el mismo principio pero teniendo en cuenta los exponentes.

💡**Ejemplo:**
$F(s) = \frac{s^{2}+2s+3}{(s+1)^{3}}$

$$ F(s) = \frac{A(s)}{B(s)} = \frac{b_{3}}{(s+1)^{3}} + \frac{b_{2}}{(s+1)^{2}} + \frac{b_{1}}{s+1} $$

$$ (s + 1)^{3} \frac{A(s)}{B(s)} = b_{3} + b_{2}(s+1) + b_{1}(s+1)^{2} $$

$$ b_{3} = (s + 1)^{3} \frac{A(s)}{B(s)} _{s=-1} = (s^{2}+2s+3) _{s=-1} = 2 $$

$$ b_{2} = \frac{d}{ds} [(s+1)^{3} \frac{A(s)}{B(s)}] _{s=-1} = [\frac{d}{ds} (s^{2}+2s+3)] _{s=-1} = (2s + 2) _{s=-1} = 0$$

$$ b_{1} = \frac{1}{2!} ( \frac{d^{2}}{ds^{2}} [(s+1)^{3} \frac{A(s)}{B(s)}] _{s=-1} = \frac{1}{2!} [ \frac{d^{2}}{ds^{2}} (s^{2}+2s+3)] _{s=-1} = \frac{1}{2} (2) = 1 $$

$$ f(t) = L^{-1}[F(s)] $$

$$ L^{-1} [\frac{2}{(s+1)^{3}}] + L^{-1} [\frac{0}{(s+1)^{2}}] + L^{-1} [\frac{1}{s+1}] $$

$$ t^{2}e^{-t} + 0 + e^{-t} $$

$$ (t^{2} + 1)e^{-t}    (t > 0) $$

## 3. Caso 3. $Q(s) tiene raíces complejas conjugadas:
$$ G(s) = \frac{P(s)}{Q(s)} = \frac{P(S)}{(s^2}+b_{1}s+c_{1})(s^2+b_{2}s+c_{2}).....(s^2+b_{n}s+c_{n}) $$

La descomposición en fracciones parciales es de la forma:

$$ G(s) = \frac{As+B}{(s^{2}+b_{1}s+c_{1}}) + \frac{Cs+D}{(s^{2}+b_{2}s+c_{2}}) + ...... + \frac{Ms+N}{(s^{2}+b_{n}S+c_{n}}) $$

Donde A, B, ...... , N coeficientes por determinar.

### 3.1. Ejercicios:

$$ \frac{2x^{2}+29x-1}{(2x+1)(x-2)^{2}} $$

$$ \frac{A}{2x+1} + \frac{B}{x-2} + \frac{C}{(x-2)^{2}} $$

$$ 2x^{2} + 29x - 11 = A(x-2)^{2} + B(2x+1)(x-2) + C(2x+1) $$

$$ 2(\frac{-1}{2})^{2} + 29(\frac{-1}{2})^{2} - 11 = A(\frac{-1}{2}-2)^{2} + B(2(\frac{-1}{2})+1)(\frac{-1}{2}-2) + C(2(\frac{-1}{2})+1) $$

$$ -25 = \frac{25}{4}A $$

$$ A = -4 $$

$$ 2(2)^{2} + 29(2) - 11 = A(2-2)^{2} + B(2(2)+1)(2-2) + C(2(2)+1) $$

$$ 55 = 5C $$

$$ C = 11 $$

$$ 2 = A + 2B $$

$$ 2 = (-4) + 2B $$

$$ 2 + 4 = 2B $$

$$ \frac{6}{2} = B $$

$$ 3 = B $$

### 3.2. Metodo resumido Caso 3.

$$ F(s) = \frac{2s + 12}{s^{2} + 2s + 5} $$

$$ s^{2} + 2s + 5 = (s + 1 + j2)(s + 1 - j2) $$

Sabiendo que este tipo de raices resulta en la suma de una funcion seno amortiguada con una coseno amortiguada

$$ L[e^{-st} sen wt] = \frac{w}{(s + a)^{2} + w^{2}} $$

$$ L[e^{-st} cos wt] = \frac{w}{(s + a)^{2} + w^{2}} $$


