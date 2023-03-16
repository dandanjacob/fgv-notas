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
## Difeomorfismo
Dados intervalos abertos $U\in\r^n$  e  $V\in\r^m$ , uma bijeção $f:U \longmapsto V$ é dita difeomorfismo quando $f$ e $f^{-1}$ são diferenciáveis.
## Reparametrização
A curva $\b(s)$ é chamada reparametrização de $\a(t): I \subset \r \longmapsto \r^2$ regular quando dados $I_0$ e um difeomorfismo $\phi(s):I_0 \longmapsto I$ temos que $\b(s) = \a( \phi(s))$ 
## Orientação de uma curva
A orientação de uma curva plana é o sentido do percurso do traço de $\a$.
Seja $\a(t)> (a,b) \longmapsto \r^2$ e $\b(s):(c,d)\longmapsto \r^2$. Daqui, $\b(s)$ é dita <u>reparametrização positiva</u> de $d$ se $\exists \phi(s):(c,d) \longmapsto (a,b)$ tal que $\phi'(s)>0 \forall c<s<d$.
Veremos agora que:
- (i) Diomorfismos preservam regularidade;
- (ii) A função comprimento de arco é um difeomorfismo;
- (iii) Toda curva regular admite reparametrização por comprimento de arco.

(i) Qualquer reparametrização de uma curva regular é regular.
Tome $\b(s) = \a(\phi(s))$, com 
$$ \left\{
\begin{matrix}
\phi(t): (c,d) \longmapsto (a,b) & t \in(a,b) \\
\phi^{-1}(s): (a,b) \longmapsto (c,d) & s \in(c,d)
\end{matrix} \right.$$
observamos que $$ \phi^{-1}(\phi(s)) =s.$$
Agora, aplicando a derivada dos dois lados dessa equação:
$$(\phi^{-1}(\phi(s)))'.\phi'(s) = 1.$$
O que implica que todas as derivações são diferentes de zero. Por outro lado, 
$$\b(s) = \a(\phi(s))$$
$$||\b'(s)|| = ||(\a(\phi(s)))'||$$
$$||\b'(s)||=||\a'(\phi(s)).\phi'(s)||$$
Observe que $\a'(\phi(s)) \neq 0$ por regularidade e $\phi(s) \neq 0$ por difeomorfismo (ou como vimos acima). Daí, $||\b'(s)|| \neq 0 \forall s \implies \b$ é regular. 
(ii) A função comprimento de arco é um difeomorfismo.
Seja $\a(t):I \longmapsto \r^2$ uma curva regular. Consideramos um ponto $t_0\in I$ e definimos a função 
$${\huge L(t)} = \int^{t}_{t_0}||\a'(u)||du, t\in I.$$
Temos, pelo Teorema Fundamental do Cálculo que $L$ é diferenciável e satisfaz
$$L'(t) = ||\a'(t)|| \neq0, \forall t \in I,$$
isto é, $L$ é uma função contínua diferenciável estritamente crescente. Em outras palavras, é uma bijeção.
O difeomorfismo de $L$ (que leva um comprimento de arco em um parâmetro) pode ser escrito como 
$$\forall s \in I_0, L(\phi(s)) =s$$
$\phi(s)$ é o parâmetro correspondente ao lugar aonde a curva tem comprimento $s$. Daí, 
$$L'(\phi(s))\phi'(s)=1$$
$$\phi'(s) = \frac{1}{L'(\phi(s))} = \frac{1}{||\a'(t)||}$$
Logo, concluimos que ela é diferenciável e $L(t)$ é difeormorfismo. 
Tomemos a função comprimento de arco que vimos ser um difeomorfismo (sendo $\phi(s)$ o lugar(ponto) correspondente) temos $L(\phi(s))=s.$
Tomando $\phi(s)$ como reparametrização, temos $(\b(s) = \a(\phi(s)))$. Derivando essa equação dos dois lados:
$$\b'(s) = \a'(\phi(s))\phi'(s) = \a'(\phi(s)). \frac{1}{||\a'(\phi(s))||} = 1$$
(iii) Toda curva regular admite reparametrização por comprimento de arco.
 (vamos nos referir à reparametrização por comprimento de arco como UNIT SPEED).
 Exemplo: expiral logaritmica.
 $$\g_k(t) = (e^{kt}cost, e^{kt}sent)$$
 $$\g_k'(t) = (e^{kt}(kcost-sent), e^{kt}(ksent+cost))$$
 $$||\a'_k(t)||^2 = e^{2kt}(k^2+1)$$
 Então a função comprimento de arco da função logaritmica é 
 $$L_0^t(\g_k) = \int_0^t\sqrt{k^2+1}e^{ku}du = \sqrt{k^2+1}(e^{tk}-1)$$
 Em particular, para $t=1$:
 $$=\sqrt{2}(e^t-1)$$
 Daí a função comprimento de arco a partir de $t=0$ é dada por $L_0^t(\gamma_1)$.
 A função a ser usada como reparametrização é a inversa da comprimento de arco, dada por 
 $$L^{-1}(s) = ln(\frac{s}{\sqrt{2}}+1)$$
 $$\bar{\g}(s) = ((\frac{s}{\sqrt{2}}+1)cosln(\frac{s}{\sqrt{2}}+1),(\frac{s}{\sqrt{2}}+1)sinln(\frac{s}{\sqrt{2}}+1) )$$
 > REPARMETRIZAÇÃO POR COMPRIMENTO DE ARCO

1 - Calcular a derivada da função r(t); 

2 - Calcular o módulo da derivada r'(t) ;

3 - Resolver a integral do módulo |r'(t)| no intervalo de tempo qualquer ;

4 - Escrever t em função de s ;

5 - Substituir na expressão inicial ;

6 - A parametrização por comprimento de arco está pronta
