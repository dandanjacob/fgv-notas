Aluno: Daniel Jacob Tonn
1) Demonstre a desigualdade de Cauchy
$$|a_1b_1 + ... + a_nb_n|^2 \leq (|a_1|^2 + ... + |a_n|^2)(|b_1|^2 + ... + |b_n|^2)$$
onde $a_j,b_j: j=1,...,n$ são números complexos.

Resposta: 
Vamos realizar a demonstração por indução.
Primeiro, vamos verificar se é válido para $j=1$:
$$|a_1b_1|^2 \leq |a_1|^2|b_1|^2$$
Sendo $a=x+iy$ e $b=w+iz$:
$$|(xw-zy)+i(yw+zx)|^2 \leq (x^2+y^2)(w^2+z^2)$$
$$(xw-zy)^2 + (yw+zx)^2 \leq (x^2+y^2)(w^2+z^2) $$
$$x^2w^2 - \cancel{2xwzy} + z^2y^2 + y^2w^2 + \cancel{2ywzx} + z^2x^2 \leq x^2w^2 + x^2z^2+y^2w^2+y^2z^2$$
$$x^2w^2 + z^2y^2 + y^2w^2 + z^2x^2 = x^2w^2 + x^2z^2+y^2w^2+y^2z^2$$
Verificada a base da nossa indução, vamos criar nossa hipótese indutiva:
$$|a_1b_1 + ... + a_kb_k|^2 \leq (|a_1|^2 + ... + |a_k|^2)(|b_1|^2 + ... + |b_k|^2)$$
Nos resta então provar para $k+1$:
$$|a_1b_1 + ... + a_{k+1}b_{k+1}|^2 \leq (|a_1|^2 + ... + |a_{k+1}|^2)(|b_1|^2 + ... + |b_{k+1}|^2)$$
Tomemos o primeiro membro da desigualdade , como a seguir:
$$|a_1b_1 + ... + a_{k+1}b_{k+1}|^2 = |(a_1b_1 + ... + a_nb_n) + (a_{k+1}b_{k+1})|^2$$
Pela Desigualdade Triangular:
$$|a_1b_1 + ... + a_nb_n + a_{k+1}b_{k+1}| \leq |a_1b_1 + ... + a_nb_n| + |a_{k+1}b_{k+1}|$$
Da nossa hipótese indutiva, temos que 
$$|a_1b_1 + ... + a_kb_k| \leq \sqrt{(|a_1|^2 + ... + |a_k|^2)}\sqrt{(|b_1|^2 + ... + |b_k|^2)}$$
Substituindo esse módulo no segundo termo da desigualdade triangular:
$$|a_1b_1 + ... + a_nb_n| + |a_{k+1}b_{k+1}| =$$ $$\sqrt{(|a_1|^2 + ... + |a_k|^2)}\sqrt{(|b_1|^2 + ... + |b_k|^2)} + |a_{k+1}b_{k+1}|$$
Daí, temos que
$$|a_1b_1 + ... + a_{k+1}b_{k+1}|^2 \leq$$ $$ (\sqrt{(|a_1|^2 + ... + |a_k|^2)}\sqrt{(|b_1|^2 + ... + |b_k|^2)} + |a_{k+1}b_{k+1}|)^2$$
Desenvolvendo essa potência:
$$ (|a_1|^2 + ... + |a_k|^2)(|b_1|^2 + ... + |b_k|^2 + |a_{k+1}b_{k+1}|^2 + $$
$$2\sqrt{(|a_1|^2 + ... + |a_k|^2)}\sqrt{(|b_1|^2 + ... + |b_k|^2)}|a_{k+1}b_{k+1}|$$
Olhando pela desigualdade de Cauchy para $k+1$, basta provarmos que (1)
$$2\sqrt{(\sum_{i=1}^{k}|a_k|^2)}\sqrt{(\sum_{i=1}^{k}|b_k|^2)}|a_{k+1}||b_{k+1}| \leq (\sum_{i=1}^{k}|a_k|^2)|b_{k+1}|^2 + (\sum_{i=1}^{k}|a_k|^2)(|a_{k+1}|^2)$$
Para quaisquer $A, B \in \r$ é válido $(A-B)^2>0 \implies A^2+B^2>2AB.$
Sendo 
$$A = \sqrt{(\sum_{i=1}^{k}|a_k|^2)}(b_{k+1})$$
$$B = \sqrt{(\sum_{i=1}^{k}|a_k|^2)}(|a_{k+1}|)$$
concluímos que (1) é verdade e portanto 
$$|a_1b_1 + ... + a_{k+1}b_{k+1}|^2 
\leq (|a_1|^2 + ... + |a_k|^2 + |a_{k+1}|^2)(|b_1|^2 + ... + |b_k|^2+|b_{k+1}|^2))$$
2) **Demonstre que $$\left| \frac{a-b}{1-\bar{a}b} \right| < 1$$ se $|a|<1$ e $|b|<1$.**
Podemos pegar o quadrado da desigualdade e tomar o módulo do denomindor e numerador da fração separadamente:
$$\frac{|a-b|^2}{|1-\bar{a}b|^2} < 1$$
Sendo $|c| = \bar{c}c$, temos:

$$\frac{(a-b)(\bar{a} - \bar{b})}{(1-\bar{a}b)(1-a\bar{b})} < 1$$
Desenvolvendo as multiplicações:
$$ \frac{a\bar{a} - a\bar{b} - b\bar{a} + b\bar{b}}{1-a\bar{b} - \bar{a}b + \bar{a}ba\bar{b}} <1$$
ou melhor, 
$$ \frac{|a|^2 - a\bar{b} - b\bar{a} + |b|^2}{1-a\bar{b} - \bar{a}b + |b|^2|a|^2} <1 $$$$ |a|^2 - a\bar{b} - b\bar{a} + |b|^2 <1-a\bar{b} - \bar{a}b + |b|^2|a|^2 $$
$$ |a|^2 + |b|^2 <1 + |b|^2|a|^2 $$
Pelo enunciado $|a|<1\implies|a|^2<1$. Podemos reescrever $1 = \frac{1-|b|^2}{1-|b|^2} > |a|^2$. Multiplicando ambos os termos da desigualdade por $(1-|b|^2)$:
$$|a|^2|1-|b|^2| < |1-|b|^2| \implies |a|^2-|a|^2|b|^2 < 1-|b|^2 $$ 
Rearranjando os termos dessa desigualdade, temos
$$|a|^2 + |b|^2 <1 + |b|^2|a|^2.$$
Concluimos portanto que $|a|^2 + |b|^2 <1 + |b|^2|a|^2$, o que implica $$\left| \frac{a-b}{1-\bar{a}b} \right| < 1.$$
3) **Represente graficamente cada um dos seguintes subconjuntos do plano complexo, com $z \in \c$:**
- $Re(1/z^2)<1/2$
- $|z-1|=Imz$
- $z^4=16$
Respostas:
(i) Seja $z=x+iy$ complexo, então $z^2 = x^2-y^2+2xyi$ e 
$$\frac{1}{z^2} = \frac{1}{x^2-y^2+i(2xy)}.$$
Multiplicando a fração pela conjugada:
$$\frac{1}{(x^2-y^2)+i(2xy)}.\frac{(x^2-y^2)-i(2xy)}{(x^2-y^2)-i(2xy)} = \frac{(x^2-y^2)-i(2xy)}{(x^2-y^2)^2+(2xy)^2}$$
$$= \frac{(x^2-y^2)-i(2xy)}{x^4+y^4+2x^2y^2} = \frac{(x^2-y^2)-i(2xy)}{(x^2+y^2)^2}.$$
Tomando apenas a parte real, temos 
$$Re(1/z^2) = \frac{x^2-y^2}{(x^2+y^2)^2}<\frac{1}{2},$$
equação essa que representa uma lemniscata, sendo os pontos de coordenadas exteriores a essa lemniscata favoráveis à desigualdade. Verificar que essa equaçãao representa o exterior de uma lemniscata não é trivial e foram utilizados recursos computacionais para exibir o domínio dessa função.
![[lemnniscata.png]]
(ii) Sendo $z=x+iy$:
$$|z-1| = \sqrt{(x-1)^2 +y^2}$$
$$Im(z) = y$$

$$\sqrt{(x-1)^2 +y^2} = y$$
$$(x-1)^2 +y^2 = y^2$$

$$(x-1)^2= 0$$
$$x=1.$$
Concluímos que o conjunto que satisfaz a igualdade é a reta $x=1$.
![[reta.png]]
(iii) Sendo $z=x+iy$ e $u=z^2$. Então $u^2=16$.
Daí,
$$u = \pm \sqrt{16}$$
$$u = \pm4$$
Se $z^2=u = +4$:
$$z=\pm \sqrt{4} = \pm 2$$
Se $z^2= u = -4$:
$$z=\sqrt{-4} = \pm 2i.$$
Logo, concluímos que o conjunto que satisfaz $z^4=16$ é 
$$\Omega =\{2,-2,2i,-2i\}$$
![[Pasted image 20230308115305.png]]

4) **Encontre a raiz quadrada de $1+\sqrt{2}i$ e a raiz cúbica de $-81$.**
(i) Sendo $z=x+iy$, complexo tal que $z^2=1+\sqrt{2}i$. 
$$(x+iy)(x+iy) = x^2-y^2+2xyi$$
Daí, 
$$\left\{
\begin{matrix}
x^2-y^2 &= 1 \\
2xy  &= \sqrt{2}
\end{matrix}\right.$$
Da segunda equação deste sistema, temos 
$$y = \frac{\sqrt{2}}{2x}.$$
Substituindo na primeira equação deste mesmo sistema:
$$x^2-\frac{2}{4x^2} = 1$$
$$4x^4-2 = 4x^2$$

$$2x^4-2x^2-1=0$$
Sendo $\bar{x} = x^2:$
$$2\bar{x}^2-2\bar{x}-1=0$$
$$\bar{x} = \frac{2\pm\sqrt{4-4.2(-1)}}{4}$$
$$\bar{x} = \frac{1\pm\sqrt{3}}{2}$$
No entanto, $\sqrt{\bar{x}}=x$.

$$x = \sqrt{\frac{1\pm\sqrt{3}}{2}}$$
Como $x \in \r$:
$$x = \sqrt{\frac{1+\sqrt{3}}{2}}.$$
Por fim, substituindo os valores de $x$ encontrados na primeira equação do sistema:
$$\frac{1+\sqrt{3}}{2}-y^2 = 1$$
$$y^2 =  \frac{1+\sqrt{3}}{2}-1$$
$$y^2 =  \frac{\sqrt{3}}{2}-\frac{1}{2}$$
$$y = \sqrt{\frac{\sqrt{3}-1}{2}}$$
Note que da segunda equação temos que o produto $xy$ é positivo, então $x$ e $y$ possuem mesmo sinal.
Logo, as soluções são 
$$z_1 =   \sqrt{\frac{1+\sqrt{3}}{2}} +  \sqrt{\frac{\sqrt{3}-1}{2}}i$$
$$z_2 =   -\sqrt{\frac{1+\sqrt{3}}{2}} -  \sqrt{\frac{\sqrt{3}-1}{2}}i$$
(ii) Sendo $z=x+iy$ uma das três raizes de $-81$:
$$\sqrt[3]{-81} = -3\sqrt[3]{3} \implies z_1 = -3\sqrt[3]{3} + 0i$$
Como visto em sala, as soluções tem mesmo módulo e formam ângulos iguais entre soluções adjacentes quando interpretadas como vetores no plano complexo. Em outras palavras, o ângulo entre duas soluções adjacentes equivale a $120º$, sendo as soluções distribuidas sobre a circunferência de raio $3\sqrt[3]{3}$, como a seguir:
![[Pasted image 20230308202754.png]]
Assim sendo, temos :
$$z_1 = 3\sqrt[3]{3}$$
$$z_2 = 3\sqrt[3]{3}(cos(60º)+isen(60º) = 3\sqrt[3]{3}(\frac{1}{2}+\frac{\sqrt{3}}{2}i)$$
$$z_3 = 3\sqrt[3]{3}(cos(60º)-isen(60º) = 3\sqrt[3]{3}(\frac{1}{2}-\frac{\sqrt{3}}{2}i)$$