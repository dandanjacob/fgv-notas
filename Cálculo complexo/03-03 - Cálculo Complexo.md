$\newcommand { \r }{ \mathbb { R }}$
$\newcommand { \c }{ \mathbb { C }}$
$\newcommand { \z }{ \mathbb { Z }}$
$\newcommand { \n }{ \mathbb { n }}$
$\newcommand { \q }{ \mathbb { q }}$
$\newcommand { \t }{ \theta}$
$\newcommand { \rh }{ \rho}$
$\newcommand { \d }{ \delta}$
## Coordenadas Polares

Seja $z \in \mathbb{C}: z=x+iy$
IMAGEM AQUI 
Cada ponto pode ser representado em coordenadas polares como $$z = r(cos\theta , sen\theta),$$ onde $\theta$ é a inclinação do vetor que representa o número e $r$ é a distância desse ponto à origem (módulo do vetor): $$r = |z| = (x^2 + y^y)^{1/2}$$   e o argumento $arg(z) = {\theta + 2\pi z}$ .
Tomando então dois números complexos expressos em coordenadas polares:
$$z = |z|(cos\theta , sen\theta)$$
$$w = |w|(cos\rho  , sen\rho)$$
Ao efetuar a multiplicação desses dois vetores temos 
$$zw = |z||w|(cos\theta + isen\theta)(cos\rho+isen\rho)$$
$$  = |z||w|(cos\theta cos\rho - sen\theta sen\rho + i(sen\rho cos\theta + sen\theta cos\rho))$$
> Nota:
> $cos(\alpha +\beta ) = cos\alpha cos\beta -sen\alpha sen\beta$
>   $sen(\alpha +\beta ) = sen\alpha cos\beta + cos\alpha sen\beta$

$$ = |z||w|(cos(\theta + \rho) + isen(\theta + \rho))$$
Em particular, para $w=z$:
$$ z^2 = |z|^2(cos2\theta + isen2\theta)$$
$$ z^n = |z|^n(cos(n\theta) + isen(n\theta))$$
<u>Fórmula de Moivre</u>
$$ (cos\theta + isen\theta)^n = cos(n\theta)+isen(n\theta)$$
Dado $a \in \mathbb{C}$, $z^n = a, a \neq0$, existe $\sqrt[n]{a} = z$?
Sendo $a,z \in \mathbb{C}$ podemos reparametrizá-los em coordenadas polares como :
$$ a = r(cos\rho + i sen\rho), r\neq 0,$$
$$ z = p(cos\theta + i sen\theta), p\neq 0,$$
Temos $$z^n = a$$
$$p^n(cos\theta+isen\theta)^n = r(cos\rho + isen\rho)$$
Pela fórmula de Moivre:
$$p^n(cos(n\theta)+isen(n\theta)) = r(cos\rho + isen\rho)$$
ou seja, $p^n = r$, $cos(n\theta) = cos\rho$, $sen(n\theta) = sen\rho$. 
Sendo assim, concluimos que $p = r^{1/n}$ e que $n\theta = \rho \implies \theta = \frac{2k\pi + \rho}{n}, k \in \mathbb{Z}.$
Note que existem infinitas soluções. Para sermos mais precisos:
$$\left\{ \begin{matrix}k=0 \implies \theta_0 = \frac{\rho}{n} & w_0 \\
k=1 \implies \theta_1 = \frac{\rho+ 2\pi}{n} & w_1\\
\vdots \\
k=n-1 \implies \theta_{n-1} = \frac{\rho+ 2(n-1)\pi}{n} & w_{n-1}\\
k=n \implies \theta_{n} = \frac{\rho+ 2(n)\pi}{n} = \frac{\rho}{n} + 2\pi& w_n\end{matrix}\right.$$
A partir de $k=n$ as soluções começam a se repetir, portanto as soluções podem ser resumidamente escritas como $S = \{w_0,w_1,...,w_{n-1}\}$
Ao representar todas essas soluções no plano, encontramos vetores de mesmo módulo e que possuem mesmo ângulo entre soluções adjacentes, formando uma polígono regular:
IMAGEM AQUI

> Exercício
> Encontre as soluções para $z^3 = 1$.
 
  Solução:
  Reescrevendo $z$ em coordenadas polares temos $z=r(cos\t+ isen\t)$. Logo, $z^3 = r^3(cos3\t + isen3\t)$, por Moivre.
  Como $z^3 = 1 = 1(1,0) =  r^3(cos3\t + isen3\t)$, $r^3 = 1 \implies r=1$ 
  $$ \left\{ \begin{matrix}
	cos3\t & =1 \\
	sen3\t & =0
   \end{matrix}
  \right.$$
  Donde $sen3\t = 0$ apenas se $3\t = k\pi$, $k \in \z \implies \t = \frac{k\pi}{3}$.
  Se $\t = \frac{k\pi}{3}$, então $cos3\t = 1$ apenas para $k = 2$, sem repetições. 
 Sendo assim, $\t = \frac{2\pi}{3}$. 
  $$\left\{ \begin{matrix} \theta_0 = \frac{2\pi}{3} & w_1 \\
 \theta_1 = 2\frac{2\pi}{3} = \frac{4\pi}{3} & w_2\\
 \theta_{2} = 3\frac{2\pi}{3} = 2\pi & w_{3}\\
 \theta_{3} = 4\frac{2\pi}{3} = 2\pi & w_4\\
 \theta_{4} = 5\frac{2\pi}{3} = \frac{4\pi}{3} + 2\pi & w_5\end{matrix}\right.$$
Note que a partir de $w_3$ as soluções começam a se repetir, portanto existem $3$ soluções, que são $\{2\pi/3; 4\pi/3 \mbox{ e } 2\pi\}$.


## Funções Complexas
Uma função complexa é uma aplicação $f:\mathbb{C} \rightarrow \mathbb{C}$  
Exemplo 1:  
$$f(z) = z/2$$
Sendo $z = x+iy$, então $f(x,y) = (x/2,y/2) = 1/2(x+iy)$.
Em particular, o círculo de raio $|z|$ é comprimido ao círculo de raio $|z|/2$. 

Exemplo 2: 
$$f(z) = i(z)$$
Sendo $z=x+iy$ então $iz = ix - y$, isto é, $f(x,y)\longmapsto (-y,x)$. Importante destacar que essa transformação é tal que leva um vetor à um vetor ortogonal.
> Exercício
> Averiguar que ângulo foi rodado o vetor na aplicação anterior.
 
Calculando o produto interno entre $x+iy$ e $ix-y$ temos:
$$<(x,y), (-y,x)> = -xy + xy = 0$$
Logo, como o produto interno é $0$, os vetores são ortogonais.

Exemplo 3: 
$$f(z) = (z+iz)/2$$
>Problema
>1)$f(z) = \lambda z$, $\lambda \in \c \backslash \{0\}$ 
>2)$f(z) = \lambda z+z^2$ 



Seja $\Omega \subset \c$ aberto e $f:\Omega \longmapsto \c$. A função $f$ é dita analítica em $\Omega$ se $\forall z \in \Omega$ 
$$ f'(z) = lim_{h\longmapsto 0}\frac{f(z+h)-f(z)}{h}$$
existir e independente da direção em que se chegue ao ponto em discussão a derivada for a mesma.
Sendo $z=x+iv$, podemos definir $f(z)=u(z)+iv(z)$ como $f(z) = u(x,y)+iv(x,y)$.
Se aproximando primeiro pela horizontal temos 
$$ f'(z) = lim_{h\longmapsto 0}\frac{f(z+h)-f(h)}{h} = \frac{\delta f}{\delta x} = \frac{\d u}{\d x}+i\frac{\d v}{\d x}, h \in \r$$
Se aproximando agora pela vertical temos $$ f'(z) = lim_{k\longmapsto 0}\frac{f(z+ik)-f(z)}{ik}$$
Multiplicando denominador e numerador por $-i$:
$$-i.lim_{k\longmapsto 0}\frac{f(z+ik)-f(z)}{k} = -i.lim_{k\longmapsto 0}\frac{f(x, y+k)-f(x,y)}{k} = -i\frac{\d f}{\d y}$$
$$ -i(\frac{\d u}{\d y}+ i\frac{\d v}{dy}) = \frac{\d v}{\d y}- i\frac{\d u}{dy}$$
Em resumo, se aproximamos pela horizontal temos$$\frac{\d u}{\d x} + i\frac{\d v}{\d x}$$
E se nos aproximamos pela vertical temos 
$$ \frac{\d v}{\d y} -i\frac{\d u}{\d y} $$
Logo, como o limite deve existir e ser igual para que a derivada exista, então 
$$ \left\{ \begin{matrix}\frac{\d u}{\d x}= \frac{\d v}{\d y} \\
\frac{\d v}{\d x} = -\frac{\d u}{\d y}
\end{matrix} \right.$$
Essas são as equações de <u>Cauchy-Riemman</u>.
Analisando $|f'(z)|^2$, temos:
$$ |f(z)|^2 = (\frac{\d u}{\d x})^2 + (\frac{\d v}{\d x})^2$$
Utilizando as equações de Cauchy-Riemman podemos reeescrever como
$$|f(z)|^2 = \frac{\d u}{\d x}\frac{\d v}{\d y} 
-\frac{\d v}{\d x}\frac{\d u}{\d y}$$
Podemos interpretar essa equação como determinante da matriz Jacobiana.
$$= det\left(\left| \begin{matrix} \frac{\d u}{\d x} & \frac{\d u}{\d y} \\ \frac{\d v}{\d x} & \frac{\d v}{\d y}\end{matrix} \right|\right)$$
A equação Laplaciana é $$\Delta u = \frac{\d^2 u}{\d x^2}+ \frac{\d^2 u}{\d y^2} .$$
Fazendo uma breve analogia com as equações de Cauchy:
$$ \frac{\d}{\d x}(\frac{\d u}{\d x})  = \frac{\d}{\d y}(\frac{\d v}{\d y})$$
$$ \frac{\d}{\d y}(\frac{\d u}{\d y})  = \frac{\d}{\d x}(\frac{\d v}{\d x}).$$
Portanto, se $$ \frac{\d}{\d y}(\frac{\d v}{\d y}) -  \frac{\d}{\d x}(\frac{\d v}{\d x}) = 0,$$
$u$ é chamada de função harmônica e satisfaza equação de Laplace $\Delta u = 0$.