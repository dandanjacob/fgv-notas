$\newcommand { \r }{ \mathbb { R }}$
$\newcommand { \c }{ \mathbb { C }}$
$\newcommand { \z }{ \mathbb { Z }}$
$\newcommand { \n }{ \mathbb { n }}$
$\newcommand { \q }{ \mathbb { q }}$
$\newcommand { \t }{ \theta}$
$\newcommand { \rh }{ \rho}$
$\newcommand { \d }{ \delta}$

### Topologia de $\c$
- Fernandez e Bernardes, cap3
Exemplos de funções holomorfas:
- $f(Z) = z^2$
Se $z=re^{i\t}$, coordenadas polares, $f(z) = r^2e^{2i\t}$
![[Pasted image 20230314101845.png]]
## Funções Lineares
$$l:\c \longmapsto \c$$
1) $l(z_1+z_2) = l(z_1)+l(z_2)$
2) $l(\lambda z) = \lambda l(z)$
3) Se $\lambda \in \c$ então $l$ é chamada $\c$-linear e caso  $\lambda \in \r$ então $l$ é chamada $\r$-linear.
4) $l(0)=l(z-z) = l(z)+l(-z)$
   $l(z)-l(z) = 0$
   $\r^2: l(x,y) = (ax+by,cx+dy)$
   Suponhamos que $l$ é $\r$-linear.
   $l(z) = xl(1)+yl(i)$
   $\a=l(1); \b=l(i)$
   $x\a+y\b = \frac{z+\bar{z}}{2}\a-i\b\frac{z+\bar{z}}{2}$
   $l(z) =  \frac{\a-i\b}{\a}z+\frac{\a+i\b}{2}\bar{z}$
   $\r$ linear com coeficientes com conjugada $az+b\bar{z} \implies \bar{a}=b$
   Suponha agora que $l$ é $\c$ linear.
   $z=1z$
   $l(z) = l(1)z=cz, c\in \c$
   Dizemos que $w=l(z)$
   $w=u+iv$
   $u+iv = (a_1+ia_2)(x+iy)+(b_1+ib_2)(x-iy)$
   $u+iv = (a_1x-a_2y+b_1x+b_2y+i(-b_1y+b_2x+a_1y+a_2x)$
   $$u = a_1x+b_1x - a_2y+b_2y$$
   $$v = -b_1y+b_2x+a_1y+a_2x$$
   $$ \begin{bmatrix}
   u \\ v 
   \end{bmatrix} = 
   \begin{bmatrix}
   a_1+b_1 & -(a_2-b_2) \\
   a_2+b_2 & a_1-b_1
   \end{bmatrix}
   \begin{bmatrix}x \\ y
   \end{bmatrix}
   $$
   $$\left( \begin{matrix} u \\ v \end{matrix} \right) = A\left( \begin{matrix} x \\ y \end{matrix} \right)$$
   ## Transformações lineares de $\r^2$
   $l(z) = az+b\bar{z}$
   $\mu(z) = az$
   > Uma transformação é tal que se o espaço estiver limitado por retas, então a transformação também está limitada por retas.
   
$\mu(z) = az$
$a = re^{i(\t+\t_0)}$ 
$z=\rho e^{i\t}$
$\mu(z) = \rho r e^{i(\t+\t_0)}$
(???)

$z(z) = z + z^2$
Vamos mudar a variável
$w=1/z$
