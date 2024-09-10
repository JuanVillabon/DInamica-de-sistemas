# Descomposicion en fracciones parciales
## 1. Caso 1. $Q(s)$ tiene raíces reales distintos:

$$ G(s) = \frac{P(s)}{Q(s)} = \frac{P(S)}{(s+p_{1})(s+p_{2})----(s+p_{n})} $$

La descomposición en fracciones parciales es de la forma:

$$ G(s) = \frac{A}{(s+p_{1})} + \frac{B}{(s+p_{2})} + ---- + \frac{N}{(s+p_{n})} $$

Donde A, B, ...... , N coeficientes por determinar.

### 1.1. Ejercicio:

### 1.2 Método resumido (Caso 1)

$$ F(s) = \frac{A(s)}{B(s)} = \frac{a_{1}}{s+p_{1}} + \frac{a_{2}}{s+p_{2}} + ...... + \frac{a_{n}}{s+p_{n}} $$

Sabiendo que $a_{k} (k=1,2,3,...)$ son constantes, $a_{k}$ puede hallarse multipicando ambos lados de la igualdad por $(s+p_{k})$ y haciendo $s = -p_{k}$, de lo cual se obtiene

$$[(s+p_{k}\frac{A(s)}{B(s)}]_{s=-pk} = $$

$$ [\frac{a_{1}}{(s+p_{1}}(s+p_{k}) + \frac{a_{2}}{s+p_{2}}(s+p_{k}) + .... + \frac{a_{k}}{s+p_{k}}(s+p_{k}) + .... + \frac{a_{n}}{s+p_{n}}(s+p_{k})]_{s=-pk} $$

Se cancelan todas menos $a_{k}$

$$ a_{k} = [(s+p_{k}) \frac{S(s)}{B(s)}]_{ s = -pk} $$

1.2. Ejercicio:


## 2. Caso 2. $Q(s)$ tiene n raíces reales repetidos:

$$ G(s) = \frac{P(s)}{Q(s)} = \frac{P(S)}{(s+p)^{n}} $$

La descomposición en fracciones parciales es de la forma:

$$ G(s) = \frac{A}{(s+p)} + \frac{B}{(s+p)^2} + .... + \frac{N}{(s+p)^n} $$

Donde A, B, ...... , N coeficientes por determinar.

### 2.1. Ejercicios:

### 2.2. Metodo resumido Caso 2.
Se puede aplicar el mismo principio pero teniendo en cuenta los exponentes.

💡**Ejemplo:**
$F(s) = \frac{s^{2}+2s+3}{(s+1)^{3}}$

$$ F(s) = \frac{A(s)}{B(s)} = \frac{b_{3}}{(s+1)^{3}} + \frac{b_{2}}{(s+1)^{2}} + \frac{b_{1}}{s+1} $$

$$ (s + 1)^{3} \frac{A(s)}{B(s)} = b_{3} + b_{2}(s+1) + b_{1}(s+1)^{2} $$

$$ b_{3} = |(s+1)^{3}\frac{A(s)}{B(s)}_{s=1}| = (s^{2}+2s+3)_{s=-1} = 2 $$

$$ b_{2} = (\frac{d}{ds}[(s + 1)^{3} \frac{A(s)}{B(s)}])_{s=-1} = [\frac{d}{ds} (s^{2} + 2s + 3)]_{s=-1} = (2s + 2)_{s=-1} = 0 $$

$$ b_{1} = \frac{1}{2!} (\frac{d^{2}}{ds^{2}} [(s + 1)^{3} \frac{A(s)}{B(s)}]_{s=-1} = \frac{1}{2!} [ \frac{d^{2}}{ds^{2}} (s^{2} + 2s + 3)]_{s=-1} = \frac{1}{2}(2) = 1 $$

$$ f(t) = L^{-1}[F(s)] $$

$$ L^{-1} [\frac{2}{(s+1)^{3}}] + L^{-1} [\frac{0}{(s+1)^{2}}] + L^{-1} [\frac{1}{s+1}] $$

$$ t^{2}e^{-t} + 0 + e^{-t} $$

$$ (t^{2} + 1)e^{-t}    (t > 0) $$

### 2.3. Ejercicio:

## 3. Caso 3. $Q(s) tiene raíces complejas conjugadas:
$$ G(s) = \frac{P(s)}{Q(s)} = \frac{P(S)}{(s^2}+b_{1}s+c_{1})(s^2+b_{2}s+c_{2}).....(s^2+b_{n}s+c_{n}) $$
La descomposición en fracciones parciales es de la forma:
$$ G(s) = \frac{As+B}{(s^2+b_{1}s+c_{1}) + \frac{Cs+D}{(s^2+b_{2}s+c_{2})} + ...... + \frac{Ms+N}{(s^2+b_{n}S+c_{n})}
Donde A, B, ...... , N coeficientes por determinar.

### 3.1. Ejercicios:

### 3.2. Metodo resumido Caso 3.

