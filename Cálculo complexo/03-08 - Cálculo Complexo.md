Dado $z_0\in \Omega$, com $\Omega \subset \c$ aberto e $f:\Omega \longmapsto \c$. Dizemos que $f$ é contínua em $z_0$ se para todo $\epsilon >0$ existe $\delta>0$ tal que se $|z-z_0|<\delta$ então $|f(z)-f(z_0)|<\epsilon$. 
Diemos que $f$ é holomorfa em $z_o \in \Omega$ se o limite 
$$\lim_{h\longmapsto0} \frac{f(z_0+h)-f(z_0)}{h} = f'(z_0)$$
existir quando $h\longmapsto0$.
>Nota
>Se tem limite é holomorfa.
>Se é expressa como uma série de função convergente é analítica.

Se $f'(z_0)$ existe, $$f(z_0+h)-f(z)-hf'(z_0) = h\Psi(h)$$
(divide por h). Aqui, $\Psi(h)\longmapsto0 \mbox{ se } h\longmapsto0$.
Logo $f$ é contínua em $z_0$.
Exemplos de funções holomorfas:
$$f(z)=z^n$$
$$\frac{(z+h)^n-f^n}{h} = \frac{(\cancel{z^n}+nz^{n-1}h+...+h^n)-\cancel{z^n}}{h} = \frac{\cancel{h}(nz^{n-1}+...+h^{n-1})}{\cancel{h}} = nz^{n-1} + h(...+h^{n-2})$$
Sabendo que $h\longmapsto0$, f$'(z) = nz^{n-1}$. 
Um exemplo de uma função que não é holomorfa é $f(z)=|z|$.
Outro exemplo de uma função não holomorfa é $f(z) = \bar{z}$. 
Demonstração: 
$$\lim_{h\longmapsto 0} \frac{\bar{(z+h)}-\bar{z}}{h} = \frac{\bar{h}}{h} $$
Se $h\in\r$ então $\lim=1$, se $h\in\c$ então $lim=-1$. Como os limites divergem, a função não é derivável e portanto não é holomorfa.
### Função exponencial
$$f(z):= 1 +z+\frac{z^2}{2!} + ... + \frac{z^n}{n!}+...$$
$$e^z:=\sum_{n=0}^{\infty}\frac{z^n}{n!}$$Essa série é absolutamente convergente, isto é, 
$$\sum_{n=0}^{\infty}\frac{|z|^n}{n!} = e^{|z|}.$$
Logo, a série é convergente e define uma função holomorfa cuja derivada $(e^z)'=e^z$.
Definimos uma série como a soma de infinitas parcelas
$$a_1+a_2+... = \sum_{n=1}^{\infty}a_n$$
Onde os somatórios parciais são 
$$s_n = a_1+a_2+...+a_n$$
$(s_n)$ é uma sequência em $\c$.
Dizemos que $$\lim_{n\longmapsto \infty}s_n = s_{\infty}$$
o questionamento é se esse limite existe.  Em outras palavras, queremos saber se dado um $\epsilon>0$, existe $n\geq n_0$ tal que  $|s_{\infty}-s_n|<\epsilon$.
Uma sequência $(a_n)$, $a_n\in\c$ é chamada sequência de Cauchy se $\forall \epsilon>0$ existir $n_0>0$ tal que se $m,n>n_0$ então $$|a_m-a_n|<\epsilon.$$
**Teorema**: Seja $a_n$ uma sequência em $\c$. Ela é convergente se, e somente se, for uma sequência de Cauchy.
Demonstração: 
Seja $A$ a convergência de $a_n$.
i) Dade $\epsilon>0$ existe $n_0>0$ tal que se $n>n_0$, então $|a_n-A|< \epsilon$. Para $m>n_0$:
$$|a_n-A-a_m+A| \leq |a_n-A|+|a_m-A| \leq \epsilon+\epsilon.$$
ii)Suponha que a sequência seja de Cauchy, então 
$$(a_n) = a_1,a_2,...,a_n$$
O limite sperior dessa sequência é $lim (sup(an)) = \alpha_n = max\{a_1,...a_n\}$. Conforme $n$ cresce, $\a_n$ também cresce.
Mostraremos que $\a_n\rightarrow A$.
Para $k>1: a_{k}, a_{k+1}, a_{k+2},..$.
A sequência $\a_n^k$ também converge para $A$. 
$$A=\lim_{n\longmapsto\infty}sup(a_n)) = \lim_{n\longmapsto\infty}A_n$$
Características: para cada $\epsilon>0$ existe $n_0>0 tal que $a_n<A+\epsilon \forall n\geq n_0$.
Daqui, $a_n < A_n <A+\epsilon$
 Lembrete: $A_n \geq A - \epsilon$ não pode acontecer.
 Existem infinitos $n\geq0$ tais que $a_n\geq A-\epsilon$ 
 $$a = \lim_{n\longmapsto0} inf(a_n)$$
 Se, e somente se, $\lim inf(a_n) = \lim sup(a_n)$ então a série converge.
 Supondo que $A\neq a$ chegamos a uma contradição.
### Série de Sequência 
$$\sum_{n=0}^{\infty}a_nz^n$$
$$S_m = \sum_{n=0}^{m}a_nz^n$$ é uma função convergente. $S_m$ convergem.
Sendo $$f_n:\Omega \rightarrow \c$$
a sequência $f_n(z_0) converge a $f(z_0)$ se $\forall \epsilon>0 \exists n_0$ tal que se $n>n_0$.
$|f_n(z_0)-f(z_0)|<\epsilon (*)$.
$f_n$ converge em $z_0\in\Omega$.
$f_n\rightarrow f$ uniformemente se $(*)$ vale para todo $z\in\Omega$. O limite de uma sequência uniforme de funções contínuas é uma função continua. Como $f_n$ é contínua em $z_0\in\Omega$. Dado $\epsilon>0$ existe $\d$ tal que se $|z-z_0|<\d$
então $|f_n(z)-f(z_0)|<\epsilon$ 
Queremos mostrar que $f$ é contínua:
Existe $n_0$ tal que se $:=|f(z)-f(z_0)| \leq |f(z)-f_n(z_0)| +|f_n(z)-f_n(z_0)|+|f_n(z_0)-f(z_0)|$
$$\leq \epsilon + \epsilon + \epsilon$$
Dizemos que $f_n(z)$ é convergente se para todo $z\in\Omega$, $(f_n(z))$ é uma sequência de Cauchy, isto é, dado $\epsilon>0 \exists n_0$ tal que $|f_n(z)-f_m(z)|<\epsilon$, para $m,n>n_0$.
#### Exemplos de séries de potências:
- $e^z=\sum_{n=0}^{\infty}\frac{z^n}{n!}$
- $1+z+z^2+...+z^n = \sum_{n=0}^{\infty}z^n = \frac{1}{1-z}$ 
- ![[Pasted image 20230309225243.png]]

$$\frac{1}{r} = \lim_{n\rightarrow\infty} sup|a_n|^{1/n}$$