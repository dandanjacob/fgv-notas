
Aluno: Daniel Jacob Tonn
1) Encontre:
- As raízes quadradas de $1-\sqrt{2}i$;
- As raízes cúbicas de $-27$;
- As raízes de ordem $5$ de $-1$;
Resposta: 
i) Sendo a raiz procurada $z=x+iy$, para $x,y \in \r$, temos:
$$z^2 = x^2-y^2 +2xyi$$
Igualando à $1-\sqrt{2}i$:
$$\left\{\begin{matrix}
x^2-y^2=1 \\
2xy = -\sqrt{2}
\end{matrix} \right.
$$
Da segunda equação, temos $x=\frac{-1}{\sqrt{2}y}$. Substituindo na primeira, obtemos 
$$\frac{1}{2y^2}-y^2 = 1 \implies 1-2y^4=2y^2$$
Realizando uma reparametrização de $u=y^2$:
$$2u^2+2u-1 = 0$$
Por Bháskara,
$$u = \frac{-1 \pm \sqrt{3}}{2}.$$
Mas como $y = \sqrt{u}$  e $y\in\r\implies y^2=u \in \r$:
$$y = \sqrt{u} = \sqrt{\frac{-1+\sqrt{3}}{2}}.$$
Substituindo o valor encontrado de $y$ na na segunda equação do sistema:
$$x^2 - \left(\sqrt{\frac{-1+\sqrt{3}}{2}}\right)^2 = 1$$
$$x^2 - \frac{-1+\sqrt{3}}{2} = 1$$

$$x^2  = 1 + \frac{-1+\sqrt{3}}{2}$$
$$x  =  \sqrt{\frac{1+\sqrt{3}}{2}}$$
Note, na segunda equação do sistema montado, que $x$ e $y$ precisam ter sinais opostos, e que isso não altera o resultado da primeira equação do sistema. 
Logo, as raízes são 
$$ z_1 =\sqrt{\frac{1+\sqrt{3}}{2}} - \sqrt{\frac{-1+\sqrt{3}}{2}}i
$$
$$ z_2 =- \sqrt{\frac{1+\sqrt{3}}{2}} + \sqrt{\frac{-1+\sqrt{3}}{2}}i
$$
ii) Sabemos que uma das raízes cúbicas de $-27$ é real e vale $-3$. Sabemos ainda que as raízes se distribuem no traço de uma circunferência de módulo $3$ e centro em $0+0i$, com ângulo entre soluções igualmente distribuídos, como na figura a seguir.
![[Pasted image 20230311224021.png]]
Podemos então escrever as soluções em coorcenadas polares como 
$$3(cos(60º) + isen(60º))$$
$$3(cos(60º) - isen(60º))$$
Note que esses vetores são conjugado um do outro.
Encontramos, então as $3$ raízes:
$$z_1 = -3$$
$$z_2 = \frac{3}{2} + \frac{3\sqrt{3}i}{2}$$
$$z_3 = \frac{3}{2} - \frac{3\sqrt{3}i}{2}$$
iii) Sabemos que uma das raízes é o número real $-1$. As outras $4$ soluções estão dispostas em um círculo de raio $1$ com ângulos de $72º$ entre sí, como na imagem abaixo:
![[Pasted image 20230311225604.png]]
Como meia volta é $\pi$, $36º$ equivalem a $\pi/5$. As soluções em coordenadas polares são:
$$z_1 = -1$$
$$z_2 = \cos(\pi/5) + i \sin(\pi/5) = \frac{1}{4}\left(1+\sqrt{5}\right)+ \left(\sqrt{\frac{5}{8}-\frac{\sqrt{5}}{8}}\right)i$$
$$z_3 = \cos(\pi/5) - i \sin(\pi/5) = \frac{1}{4}\left(1+\sqrt{5}\right)- \left(\sqrt{\frac{5}{8}-\frac{\sqrt{5}}{8}}\right)i$$
$$z_4 = \cos(3\pi/5) + i \sin(3\pi/5) = \frac{1}{4}\left(1-\sqrt{5}\right)+ \left(\sqrt{\frac{5}{8}+\frac{\sqrt{5}}{8}}\right)i$$
$$z_5 = \cos(3\pi/5) - i \sin(3\pi/5)= \frac{1}{4}\left(1-\sqrt{5}\right) -\left(\sqrt{\frac{5}{8}+\frac{\sqrt{5}}{8}}\right)i$$
2)  Sejam $f:\Omega \longmapsto \c$, $g:\Omega \longmapsto \c$  funções definidas num aberto $\Omega\subset \c$. Se $f$ e $g$ são limitadas num subconjunto $K\subset \Omega$, então $f+g$ e $f.g$ tmbém são limitadas em $K$.

Resposta:
i) Se a sequência $f$ é limitada num subconjunto $K$, podemos afirmar a existência de $M$ de forma que $M \geq|f(n)|\forall n \in K$. De forma semelhante tomemos $N$ de modo que $N \geq |g(n)|\forall n\in K$. Somando as duas desigualdades temos 
$$M+N \geq |f(n)| + |g(n)|$$
Pela desigualdade triangular, temos:
$$M+N \geq |f(n)| + |g(n)| \geq |f(n) + g(n)|$$
Sendo $R = M+N$ temos $R\geq|f(n)+g(n)|$, portanto $f+g$ é limitada.

ii) Tomando $M$ e $N$ da mesma maneira que anteriormente, temos
$$MN \geq |f(n)||g(n)| = |f(n)g(n)|$$
Tomando agora $R = MN$, temos $f.g$ limitada.

De maneira menos informal e mais geométrica, como  $f$ é limitada podemos afirmar que todos os seus elementos estão dentro de uma circunferência de raio $M$ - e da mesma forma podemos tomar uma circunferência de raio $N$ que englobe todos os elementos de $g$.
Essa ideia é formalizada por 
$$M>|f(n)|\forall n\in K$$
$$N>|g(n)|\forall n\in K$$
Ao somar ambas expressões surge do lado direito da inequação algo que é maior ou igual ao módulo de qualquer elemento de $f+g$ - conclusão tirada da desigualdade triangular. Mas se é possível limitar os elementos de $f+g$ por um módulo, então os elementos de $f+g$ estão contidos em uma circunferência de raio $M+N$.
	$$M + N>|f(n)|+|g(n)| \geq|f(n)+g(n)|\forall n\in K$$
Se agora multiplicarmos ambas equações, temos
$$MN > |f(n)||g(n)| = |f(n)g(n)|$$
Conseguimos novamente limitar $fg$ a uma circunferência, dessa vez de raio $MN$, portanto $fg$ é também limitada.


3) Determine a imagem do triângulo com vértices em $3+4i$, $3-4i$ e $-5i$ pela função $f(z) = z+5i$.
Seja $z=x+iy$, então a função $f(z) = z+5i = x + (5+y)i$ é tal que leva cada ponto do plano $5i$  acima. 
Dado o domínio  como sendo o triângulo de vértices $3+4i$, $-3+4i$ e $-5i$ (cinza), a imagem após aplicada a função é o triângulo de vértices $3+9i$, $-3+9i$ e $0 + 0i$ (verde), como representado na imagem abaixo:
![[Pasted image 20230311234323.png]]

4) Toda sequência limitada de números complexos possui uma subsequência convergente.

Resposta: 
Para que uma sequência $(z_n)$de números complexos seja convergente precisamos que $Re(z_n)$ seja convergente, assim como  $Im(z_n)$ também seja convergente. Como $(z_n)$ é limitada, então as sequências $Re(z_n)$ e $Im(z_n)$ também o são.
Como $Re(z_n)$ e $Im(z_n)$ são  sequências de números reais, podemos utilizar o teorema de *Bolzano Weiertrass* para demonstar que $(z_n)$ converge.
**Teorema de Bolzano Weiertrass**
Seja uma sequência de números reais denominada como $(a_n)$ e um pico definido como $a_n > a_m$ para qualquer $m>n$. 
Vamos dividir a demonstração em dois casos distintos: 
1) A sequência possui uma quantidade infinita de picos e sejam esses nomeados como $P_1>P_2>P_3>...$, então tomando os elementos  $(a_{n_k})$ de $(a_n)$ de modo que $(a_{n_k})$ seja um pico, então temos uma sequência monótona decrescente - e limitada - e portanto convergente. 
2) A sequência possui uma quantidade finita de picos. Então a partir de algum $n>n_0$ temos $a_n>a_{n_0}$, e para algum $m>n$ temos $a_m>a_n$ e assim por diante. Tomando os elementos  $a_{n_k}$ a partir do ultimo pico, tais que $a_{n_k}<a_{n_{k+1}}$ (afirmamos a existência desse $a_{n_{k+1}}$), temos uma sequência monótona crescente e limitada, e portanto convergente. 
Vamos chamar de $x_0$ o $\lim_{n\to \infty} (a_{n_k})$. 
Agora, sendo $(z_{n_k})$ a subsequência limitada tal que $Re(z_{n_k})$ converta a $x_0$, temos que toda subsequência de $Re(z_{n_k})$ converte também a $x_0$. Podemos tomar os elementos $(z_{n_{k_l}})$ de $(z_{n_k})$ de modo que $Im(z_{n_k})$ converta a $y_0$. Pelo Teorema de Bolzano, se $(a_n) = Im(z_{n_k})$, podemos afirma a existência de $(a_{n_k}) = Im(z_{n_{k_l}})$ de modo que $Im(z_{n_{k_l}})$ seja convergente.
Logo, concluímos que uma sequência limitada qualquer  $(z_n)$ de números complexos possui uma subsequência $(z_{n_{k_l}})$ convergente à $z_0 = x_0 + iy_0$.



$\newcommand { \r }{ \mathbb { R }}$
$\newcommand { \c }{ \mathbb { C }}$
$\newcommand { \z }{ \mathbb { Z }}$
$\newcommand { \n }{ \mathbb { N }}$
$\newcommand { \q }{ \mathbb { q }}$
$\newcommand { \t }{ \theta}$
$\newcommand { \rh }{ \rho}$
$\newcommand { \d }{ \delta}$
$\newcommand { \b }{ \beta}$
$\newcommand { \a }{ \alpha}$
$\newcommand { \g }{ \gamma}$