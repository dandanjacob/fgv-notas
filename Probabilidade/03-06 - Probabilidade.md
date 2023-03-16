<u>Bibliografia</u>
Livro Barry James - Prob: um curso em nível intermediário
Conteúdos a serem abordados:
1) Modelos probabilísticos - prob condicional e independência
2) Variáveis aleatórias e funções de distribuição
3) Esperança matemática. Integral de Stieltys
4) Distribuição e esperança condicional
5) Lei dos Grandes Números
6) Teorema Central do Limite

A origem da probabilidade se dá em jogos de azar, como:
- Lançamento de dados ou moedas, cartas, bolas em urnas, etc.
- Todos modelos equprováveis.
Chamamos de $\Omega$ o espaço amostral (conjunto dos resultados possíveis).
$$\Omega = \{w_1,w_2,...,w_n\}$$
Exemplo 1: lançamento de um dado
$$\Omega = \{1,2,3,4,5,6\}$$
Subconjuntos desse elemento são chamados de evento.Ex:
$$\mbox{evento(sair par)} = \{2,4,6\}$$
Probabilidade de um evento:
$$P(A)=\frac{n(A)}{n(\Omega)} = \frac{\mbox{nº casos favoraveis}}{\mbox{nº casos possiveis}}$$
$$P(\mbox{sair par})=\frac{n(\mbox{sair par})}{n(\Omega)} = \frac{n\{2,4,6\}}{n\{1,2,3,4,5,6\}} = \frac{3}{6} = \frac{1}{2}$$
Exemplo 2:
$5$ sorvetes são distribuídos "ao acaso" entre $10$ pessoas, das quais $2$ só gostam de morango  e $3$ somente de chocolate. Qual a probabilidade de todas ficarem satisfeitas?
Solução:
Suponha que vamos distribuir os sorvetes para as pessoas que querem morango. Da primeira pessoa à receber o sorvete, existem 5 casos favoráveis de todos os 10 casos possíveis. A segunda pessoa, no entanto,só tem a opção de 9 sorvetes, dos quais apenas 4 são de morango. Dentre as pessoas que gostam de chocolate, a primeira pode receber 5 dentre os 8 sorvetes restante, a segunda que só quer morango recebe um dos 4 entre os 7 restantes e a ultima pessoa exigente pode receber 3 dos 6 restantes. as demais pessoas podem receber qualquer sorvete. Sendo assim,
$$\frac{5}{10}.\frac{4}{9}.\frac{5}{8}.\frac{4}{7}.\frac{3}{6}. \frac{5!}{5!} = \frac{5}{126}$$
O número de subconjuntos de $p$ elementos de  um conjunto com $n$ elementos é
$$\left(\begin{matrix} n \\ p \end{matrix} \right) = \frac{n(n-1)...(n-(p-1))}{p!} = \frac{n!}{p!(n-p)!}$$
Exemplo 3:
Moeda honesta é lançada 3 vezes. Qual é a probabilidade de saírem 2 caras e 1 coroa?
Vamos pensar primeiro no total de casos possíveis. Existem duas opções de resposta pra cada lançamento,coroa(C) ou cara(K) o que significa $2.2.2 = 8$ resultados possíveis.
Agora, imagine que no primeiro lançamento saiu C. É necessário que saia apenas uma cara dentre os próximos lançamentos. Pode acontecer de sair KC ou CK. Agora, caso no primeiro lançamento saia K, é necessário que nos dois seguintes lançamentos caiam CC. Ou seja, existem 3 casos favoráveis dentre os 8 casos possíveis. Logo, a probabilidade é de $3/8$.

De forma mais geral, dado um espaço amostral $\Omega$ finito ou infinito enumerável,
$$\Omega = \{w_1,w_2,...,w_n\}$$
Definimos $p_i =$ probabilidade de sair resultado $w_i$.
$$(p_i\geq0, \forall i, p_1+p_2+p_3+...+p_n = 1$$
$$P(A) = \sum_{w_i\in A}p_i$$
Um espaço de probabilidade amostral é uma tripla $(\Omega,A,P)$ onde $\Omega$ é o espaço amostral, $A$ é uma álgebra (ou $\sigma$-álgebra) de subconjuntos de $\Omega$(conjunto de enventos aleatórios).
$P:A\longmapsto \r$ é uma medida de probabilidade.
$$$$
