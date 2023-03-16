$\newcommand { \r }{ \mathbb { R }}$
$\newcommand { \c }{ \mathbb { C }}$
$\newcommand { \z }{ \mathbb { Z }}$
$\newcommand { \n }{ \mathbb { n }}$
$\newcommand { \q }{ \mathbb { q }}$
$\newcommand { \t }{ \theta}$
$\newcommand { \rh }{ \rho}$
$\newcommand { \d }{ \delta}$
$\newcommand { \b }{ \beta}$
$\newcommand { \a }{ \alpha}$
$\newcommand { \g }{ \gamma}$
Em $\r^2$ podemos representar o parordenado $(v,u)$, com $u=(x_u,y_u)$ e $v=(x_v,y_v)$ como 
$$\begin{bmatrix}v & u\end{bmatrix} = \begin{bmatrix}x_v & x_u \\ by_v & y_u \end{bmatrix}$$
Sabemos que o determinante dessa matriz é dado por 
$$det\begin{bmatrix}x_v & x_u \\ by_v & y_u \end{bmatrix} = x_vy_u - x_uy_v.$$
Definimos a matriz de rotação de $90º$ no sentido antihorário como 
$$J = \begin{bmatrix}0&-1 \\1&0\end{bmatrix}.$$
Sendo assim, uma rotação de $90º$ no sentido antihorário do vetor $v$ equivale a:
$$\begin{bmatrix}0&-1 \\1&0\end{bmatrix}\begin{bmatrix}x_v \\y_v \end{bmatrix} = \begin{bmatrix} -y_v \\ x_v \end{bmatrix}.$$
Daí, $$det\begin{bmatrix} J_v & u\end{bmatrix} = \begin{bmatrix} -y_v \\ x_v \end{bmatrix}\begin{bmatrix}x_u & y_u\end{bmatrix} = -y_vy_u - x_ux_v = -<v,u>.$$
Já vimos na aula passada que toda curva regular admite reparametrização por comprimento de arco (unit-speed), ou seja, 
$$||\a'(t)|| = 1$$
Vamos observar que o traço produzido por uma função
$$\gamma(t):I\longmapsto\r^2 \mbox{ tal que }||\gamma(t)||=1 \forall s\in I$$
é uma curva contida na circunferência em $\r^2$ de raio $1$ e centro na origem. Vamos escrever $\gamma(t):I \longmapsto S'$, para $S'$ sendo essa circunferência de raio 1 centrada na origem.
Já vimos que quando $||\g(t)||=1$   temos $\g'(t)\bot \g(t) \forall t.$
### Função Ângulo
Dada uma função diferenciável $\g:I\longmapsto S'$ diz-se que $\t(s)$ é uma função ângulo quando $\g(s) = (cos\t(s), sen\t(s))$.
$$\t'(s) = det<\g(s),\g'(s)>$$
$$\t'(s) = det<\a'(s),\a''(s)>$$
Vamos supor que $\g(s):I\longmapsto S'$ admite ângulo diferenciável $\t(s):I\longmapsto\r$. Nesse caso temos
$$\g(s) = (-\theta(s)sen\t(s), \t'(s)cos\t(s))$$
$$ = \t'(s)(-sen\t(s),cos\t(s))$$
$$= -\t'(s)J(\g(s))$$
$$<J\g(s),\g'(s)> = <J\g(s), \t'(s)J\g(s)>$$
$$ = \t'(s)<J\g(s),J\g(s)>$$
então $$\t'(s) = det<\g(s),\g'(s)>$$
$$=det<\a'(s),\a''(s)>$$
note a parametrização unit-speed!
$$K(s) = \t'(s) = det(T(s)T'(s)) = det(\a'(s),\a''(s))$$
Em particular, $|K(s)|$ é a área do retângulo determinado pelos vetores $\a'(s)$ e $\a''(s)$.  Uma vez que $||\a'(s)||=1$, temos que $||\a''(s)||$.