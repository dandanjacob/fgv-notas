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
Vimos anteriormente que $\r$ é um corpor fechado por soma e multiplicação e possui uma relação de ordem. Ser fechado por soma e multiplicação significa que uma função $f$ é bijetiva de modo que $f:\r\times \r\longmapsto \r$, pode ser definida por $f(a,b) = a+b \longmapsto \r$ ou então $f(a,b) = ab \longmapsto \r$.
Pelos axiomas da aula anterior, podemos provar todas as propriedades, e uma propriedade já provada pode ser usada pra provar alguma outra propriedade. Sendo assim,
- 1ª Propriedade:
	Se $x,y \in\r^+$, então $x+y\in\r^+$.
	Se $x,y \in \r^+$, então $xy \in \r^+$.
- 2ª Propriedade (tricotomia):
	Ou $x=0$, ou $x\in\r^+$  ou $-x\in\r^+$. 
	Definimos então $\r^- = \{x\in\r^+:-x\in\r^+\}$.
	Definimos também $\r = \r^+\cup\r^-\cup\{0\}$.
- 3ª Propriedade:
 i) x(-y) = (-x)y
	 Prova: 
	 $$0=0$$
	 $$x(y-y) = 0$$
	 $$x(y-y)+y(-x) = +y(-x)$$
	 $$x(y)+x(-y)+y(-x) = +y(-x)$$
	 $$x(y)+y(-x)+x(-y) = +y(-x)$$
	 $$x(y)+y(-x)+x(-y) = +y(-x)$$
	 $$y(x+(-x))+x(-y) = +y(-x)$$
	 $$0+x(-y) = y(-x)$$
ii)(-x)(-y) = xy
$$0=0$$
$$x(y-y) = -y(x-x)$$
$$x(y) + x(-y) = -y(x) + (-y)(-x)$$
Vimos que $x(-y) = (-x)(y)$
$$x(y) = (-y)(-x)$$
- 4ª propriedade:
 Se $x\neq0$ então $x^2\in\r^+$.
 Pela primeira propriedade, se $x\in\r^+$,  $xx>0.$ 
 Provamos na terceira propriedade que $xx=(-x)(-x)$, portanto  $(-x)(-x)>0$, cqd.

- 5ª Propriedade: 
 $1>0$
 $1=1.1=1^2 >0$

- 6ª Propriedade:
 i) Se $x<y$ e $y<z$, então $x<z$ (propriedade transitiva).
 ii) Dado x,y ou $x<y$, ou $x=y$ ou $x>y$ (tricotomia).
 iii) Se $x<y$, $x+z<y+z \forall z \in\r$
 iv) Se $x<y$ então $z\in\r^+ \implies xz<yz$ e $z\in\r^- \implies xz>yz$.
 Provas: 
 i) $x<y \implies y-x \in \r^+$ da mesma forma que $y<z \implies z-y \in \r^+$ 
Somando dois números positivos temos um números positivo, então 
$$(y-x)+(z-y)\in\r^+$$ $$z-x\in\r^+$$
$$z>x$$
ii) sai pela tricotomia
iii) $x<y\Leftrightarrow y-x \in\r^+$
 $$y-x+z-z \in \r^+$$
 $$(y+z)-(x+z) \in\r^+$$
 $$y+z>x+z$$
 ### Origem dos naturais ($\n$) 
 O conjunto dos números formados por 1,1+1,1+1+1,... é chamado de conjunto dos números naturais e segue a propriedade de ordem.
 Seja $$0<1$$
 $$0+1<1+1$$
 $$0<1<1+1$$
 Por transitividades, $$1+1<1+1+1$$
 Denotamos essas somas por $\{1,2,3,...\}$.
 Daqui, conseguimos concluir ainda que $\n$ é infinito.
 Definimos como $\z = \n \cup -\n \cup \{0\}$
 Dado $x\in\r$:
 $$|x| = \left\{\begin{matrix}  x & se & x\in\r^+ \\
 0 & se & x = 0 \\
 -x & se & x\in\r^-  \end{matrix} \right.$$
 Ou então 
 $$|x| = max\{-x,x\}$$

  **Teorema:** $x,y \in \r$ (desigualdade triangular)
  $$|x+y|\leq |x|+|y|$$
  Temos que $|x|\geq x$ e $|y|\geq y$, daí $|x|+|y|\geq x+y$. 
  Temos ainda que $|x|\geq-x$ e $|y| \geq -y$, daí $|x|+|y| \geq -(x+y)$.
  Sendo assim, $|x|+|y| \geq max\{(x+y),-(x+y)\} = |x+y|$
  Se $a<b$ o intervalo entre $a$ e $b$ é tal que 
i) $[a,b]:x\in\r:a\leq x\leq b$  
ii) $(a,b]:x\in\r:a< x\leq b$  
iii) $[a,b):x\in\r:a\leq x< b$
iv) $(a,b):x\in\r:a< x< b$
Um conjunto $A\in\r$ é limitado superiormente se $\exists b\in\r | x\leq b$.
No caso de existência, $b$ é cota superior.
Um conjunto $A\in\r$ é limitado inferiormente se $\exists c\in\r | x\geq c$.
No caso de existência, $b$ é cota superior.
Dizemos que $A$ é limitado se for simultaneamente limitado superiormente e inferiormente.
Daí, tiramos a concllusão que $A$ é limitado se, e somente se, existir um conjunto $[c,b]$ tal que $A\in[c,b]$.
A é limitado se $\exists \d$ tal que $|x|\leq \d \forall x \in A$.
O corpo dos reais é o único corpo ordenado completo.