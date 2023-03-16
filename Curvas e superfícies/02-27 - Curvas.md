$\newcommand { \r }{ \mathbb { R }}$
$\newcommand { \c }{ \mathbb { C }}$
$\newcommand { \z }{ \mathbb { Z }}$
$\newcommand { \n }{ \mathbb { n }}$
$\newcommand { \q }{ \mathbb { q }}$
$\newcommand { \t }{ \theta}$
$\newcommand { \rh }{ \rho}$
$\newcommand { \d }{ \delta}$
Um dos objetivos do estudo de curvas é encontrar o quanto uma curva se inclina (se curva), o que nos fornece essa curvatura é o ângulo entre a função e a sua derivada.
Encontramos o valor do ângulo entre dois segmentos de reta através da <u>Lei dos cossenos</u>:
$$a² = b² + c² - 2cos\theta,$$
onde os segmentos podem ser interpretados como vetores:
$$||u-v||² = ||u||^2 + ||v||² - 2||u||||v||cos\theta ,$$
ou melhor, 
$$cos\theta = \frac{<u,v>}{||u||||v||}$$
O <u>Produto interno</u> é uma função $f:\mathbb{V}\times\mathbb{V} \rightarrow \mathbb{R}$ em um espaço vetorial (real) $\mathbb{V}$, linear em cada variável. Essa função $f$ pode ser simétrica, antissimétrica ou positiva.
- Simétrica: $f(x,y) = f(y,x)$
- Anti-simétrica: $f(x,y) = -f(y,x)$
- Positiva: $f(x,x)>0, x\neq0$
> **Exercício**
> O produto interno é uma forma bilinear simétrica, positiva e definida. 

Sejam $u = (x_1,x_2,...,x_n)$ e $v = (y_1,y_2,...,y_n)$ vetores em $\mathbb{R}^n$, segue que
$$<u,v> = x_1y_1 + x_2y_2+...+x_ny_n = y_1x_1 + y_2x_2+...+y_nx_n = <v,u>,$$
ou seja, simétrico. AQUI! (POSITIVA DEFINIDA)
A <u>Norma euclidiana</u> associa cada vetor a um número real:
$$ ||x|| = \sqrt{x_1^2 + x_2^2 + ... + x_n^2} $$
A <u>Distância euclidiana</u> é a distância entre dois pontos, em que é aplicado o teorema de pitágora recorrentemente.
$$d(x,y) = ||x-y||$$
Uma <u>parametrização</u> em $\mathbb{R}^n$ é uma aplicação $\Gamma:I \rightarrow \mathbb{R}^n$, sendo $I$ um intervalo aberto.
A curva parametrizada pode ser expressa em coordenadas em função de uma variável externa:
$$t \in I \rightarrow \Gamma(t): (\Gamma_1(t),\Gamma_2(t),...,\Gamma_n(t))$$
Exemplo:
Circunferência de raio $1$ em $\mathbb{R}^2$:
$$\Gamma(t) = (cos(t),sen(t))$$
Mola  de raio 1 em $\mathbb{R}^3$:
$$\Gamma(t) = (cos(t),sen(t),t)$$
O conjunto imagem da função parametrizada é chamada de <u>traço</u>.
Seja $\Gamma: I \rightarrow \mathbb{R}^n$ uma aplicação com $\Gamma(t) = (\Gamma_1(t)+ ... + \Gamma_n(t))$, o vetor $\Gamma'(t) = (\Gamma'_1(t)+ ... + \Gamma'_n(t))$ é chamado de vetor tangente de $\Gamma$ em $t$, ou vetor velocidade.
Em uma curva parametrizada diferenciável, dizemos que essa curva é regular se $\Gamma'(t) \neq0$, $\forall t \in I$
Exemplo:
$$ \Gamma(t) = (t^3, t^2)$$
$$\Gamma'(t) = (3t^2, 2t)$$
Para $t=0$, $\Gamma'(t) = 0$. 
Podemos determinar a reta tangente à curva em $t$ a partir do ponto $t$ e do vetor velocidade:
$$r(\lambda) = \Gamma(t)+\lambda\Gamma'(t)$$
As curvas regulares podem ser medidas integrando o módulo do vetor tangente. O comprimento da curva é dado pela noção de aproximação poligonal levada ao limite. A regularidade é essencial nesse conceito. Seja $\Gamma: I \subset \mathbb{R}^2$ uma curva regular. Vamos considerar uma partição do intervalo $[a,b]$: $P = {t_0,t_1,...t_{n-1}, t_n} \subset [a,b]$ com $a={t_0 \leq t_1 \leq t_n}$. A união de todos os segmentos $[\Gamma(t_{i-1}); \Gamma(t_{i})]$ é uma linha poligonal e seu comprimento é 
$$ {\huge{L}}_a^b(\Gamma, P) = \sum_{i=1}^n ||\Gamma'(t_i) - \Gamma'(t_{i-1})||$$
Vrifica-se que $L$ é limitada e satisfaz 
$$sup L_a^b(\Gamma, P) = \int_a^b||\Gamma'(t)||dt$$
Exemplo:
Expiral logarítmica
$$\Gamma(t) = (e^{kt}cos(t), e^{kt}sen(t))$$
onde $k$ é constante diferente de zero
O vetor tangente é 
$$\Gamma(t) = (e^{kt}(kcos(t)-sen(t)), e^{kt}(ksen(t)-sen(t)))$$
Daí, o tamanho do vetor tangente é  
$$||\Gamma'(t)||^2 = e^{2kt}(kcost-sent)^2 + e^{2kt}(cost+ksent)^2$$
$$ = (k^2+1)e^{2kt}$$
Concluimos então que o comprimento da espiral é dado por 
$$ {\huge{L}}_0^t(\Gamma_k) = \int_0^t \sqrt{k^2+1}e^{ku}du = \frac{\sqrt{k^2+1}}{k}(e^{kt}-1)$$
Em particular, para $k=1$:
$$ {\huge{L}}_0^t = \sqrt{2}(e^t-1)$$

