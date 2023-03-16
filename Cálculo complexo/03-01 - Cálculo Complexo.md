
<u>Bibliografia:</u>
- Introdução às funções de uma variável complexa (textos universitários - SBM) - Cecília Fernandez e Nilson Bernardes
- Complex Analysis - Ahlfors, Shabat - Edição MIR
- Stein+ angluém
## Números Complexos:
Os números complexos são escritos da forma  $z = x+iy$ , com $x,y \in \mathbb{R}$ e $i^2 = -1$, sendo $x$ a parte nomeada de parte real e $y$ a parte imaginária de $z$. O conjunto que contém todos os números complexos é nomeado de $\mathbb{C}$. 
o conjunto dos números imaginários é um corpo algebricamente fechado, isto é,  em qualquer polinômio de uma variável e grau dessa variável maior ou igual a 1![1](https://wikimedia.org/api/rest_v1/media/math/render/svg/92d98b82a3778f043108d4e20960a9193df57cbf), com coeficientes nesse conjunto, tem uma raiz nesse mesmo conjunto.
O corpo dos complexos é fechado por soma e multiplicação, assim como $\mathbb{R}$.
<u>Soma</u>
Sejam $z = x+iy$ e $w = u + iv$, então 
$$ z+w = (x+iy) + (u+vi) = (x+u) + i(y+v).$$
<u>Produto</u>
Sejam $z$ e $w$ definidos como anteriormente, então:
$$(x+iy)(u+iv) = xu + ixv + iyu -yv = (xu-yv) + i(xv+yu)$$
O corpo dos complexos mantém as propriedades de comutação, elemento neutro da soma e da multiplicação, existência do oposto e existência de inverso.
<u>Comutação:</u> $$ z+w = (x+iy) + (u+vi) = (x+u) + i(y+v) = w+z.$$
<u>Elemento neutro (+):</u> $$z+0 = 0+z = z$$
<u>Elemento neutro (.):</u>
Definimos a unidade no conjunto dos complexos como $1 = 1 + i0$, então $$z.1 = 1.z = z$$
<u>Oposto:</u>
Sendo $z=x+iy$, com $z\neq0$, definimos $-z = -x-iy$ e
$$ z+(-z) = 0$$
De fato, $$z+(-z) = x+iy -x-iy = (x-x) + i(y-y) = 0+i0 = 0$$
<u>Inverso:</u>
Para todo $z\neq0$, com $z=a+bi$, existe $w$ tal que $wz=1$.
Seja $w=(x+iy)$, então 
$$zw = (a+bi)(x+iy) = 1$$
$$ xa - yb + iay + ibx = 1$$
$$ (xa-yb)+(ay+bx)i = 1$$
Como a unidade nos complexos é definida como $(1+0i)$, segue que 


$$\left\{\begin{matrix}xa-yb = 1 \\ ay +bx = 0 \end{matrix} \right.$$
Podemos escrever esses sistema em notação matricial:
$$ \begin{bmatrix} a & -b \\ b & a \end{bmatrix}\begin{bmatrix} x \\ y \end{bmatrix} = \begin{bmatrix} 1 \\ 0 \end{bmatrix},$$
$$Ax=b$$
Multiplicando ambos os termos pela inversa de $A$, temos:
$$A^{-1}Ax = A^{-1}b,$$
ou melhor, $$x = A^{-1}b$$
Sendo $\Delta = det(A) = \frac{1}{a^2+b^2}$ inversa de $A$ é $$\frac{1}{\Delta}\begin{bmatrix}a & b \\ -b & a \end{bmatrix}$$
Logo, 
$$ \begin{bmatrix} x \\ y \end{bmatrix} = \frac{1}{a^2+b^2} \begin{bmatrix} a & b \\ -b & a \end{bmatrix}\begin{bmatrix} 1 \\ 0 \end{bmatrix} = \begin{bmatrix} \frac{a}{a^2+b^2} \\ \frac{-b}{a^2+b^2} \end{bmatrix}$$ Portanto, 
$$ w = x+iy = \frac{a}{a^2+b^2} + \frac{-b}{a^2+b^2}i = \frac{1}{a^2+b^2}(a-bi).
$$
$$w = \frac{1}{a^2+b^2}(a-bi).$$
### A geometria da coisa
- A parte real de $z$ é $x$ e $z$ é real quando $y=0$.
- A parte imginária de $z$ é $y$ e $z$ é puramente imaginário se $x\neq0$.
- $z$ é real e imaginário simultaneamente apenas quando $z=0$.
Os números complexos podem ser representados em um plano cujo eixo das abcissas é o eixo $x\in \mathbb{R}$ e o eixo das ordenadas é $iy, y\in \mathbb{R}$.
Definimos a <u>conjugada</u> de $z = x+iy$ como $\bar{z} = x-iy$, onde 
$$ x = \frac{1}{2}(z + \bar{z}) \mbox{ e } y = \frac{1}{2i}(z-\bar{z})$$
Segue que $\bar{z+w} = \bar{z} + \bar{w}$ e que $\bar{zw} = \bar{z}\bar{w}$.
Uma aplicação da conjulgada é, dado uma equação na forma
$$ \begin{equation}C_0z^n + C_1z^{n-1} + ... +C_{n-1}z + C_n = 0\end{equation}, (1)$$
com raiz $\zeta$, a conjugada 
$$\bar{C}_0\bar{z}^n + \bar{C_1}\bar{z}^{n-1} + ... +\bar{C_{n-1}}z + \bar{C_n} = 0 (2)$$
possui raiz $\bar{\zeta}$  que é também solução de (1).
Definimos $$|z|^2 = z\bar{z}$$ como módulo de $z$, onde $|z|^2 = x^2+y^2.$
$|z|$ pode ser interpretado como o tamanho de $z$:
$$|z| = r = \sqrt{x^2+y^2}$$
O módulo de uma soma $|a+b|^2$ é $|a|^2+|b|^2 + 2Rea\bar{b}$ e o módulo da subtração é
$|a-b|^2 = |a|^2+|b|^2 - 2Rea\bar{b}$. Somando as duas equações, temos $|a+b|^2 + |a-b|^2 = 2(|a|^2 + |b|^2)$.
Podemos afirmar que $|z|^2 = x^2 + y^2 \geq x^2 = (-x)^2$, d'onde 
$$ -|z| \leq Rez \leq |z|.$$
De forma semelhante, 
$$ -|z| \leq Imz \leq |z|$$
Agora, redefinindo a igualdade $|a+b|^2=|a|^2+|b|^2 + 2Rea\bar{b}$ para $|a+b|^2\leq|a|^2+|b|^2 + 2Rea\bar{b}$, chegamos na Desigualdade Triangular:
$$ |a+b| \leq |a| + |b|$$
Essa desigualdade se torna igualdade apenas para $Rez =|z| \geq 0 \mbox{ e } z\in\mathbb{R}$.
Se $Rez = |z|$ é real positiva, então $\frac{b}{b}a\bar{b} = \frac{a}{b}|b|^2 \implies \frac{a}{b}>0$
