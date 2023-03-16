$\newcommand{\A}{\mathbb{A}}$
$\newcommand{\o}{\Omega}$
Como deve ser a coleção $\mathbb{A}$ dos subconjuntos de $\Omega$ aos quais vai se atribuir probabilidade?
1) $\o \in \A$ (para poder escrever $P(\o)=1$);
2) $A \in \A \implies A^c=\o-A\in\A$ (para poder escrever $P(A^c)=1-P(A)$);
3) $A,B \in \A \implies A\cup B\in\A$  (para poder escrever $P(A\cup B) = P(A)+P(B)$, quando $A$ e $B$ disjuntos.
Consequências:
$$A,B,C \in \A \implies A\cup B\cup C \in \A$$
$$A_1,...,A_n \in \A \implies A_1\cup A_2 \cup ... \cup A_n \in \A$$
$$A,B \in \A \implies A\cap B \in \A$$
Em particular $$A\cap B = (A^c\cup B^c)^c$$
$$A_1,...,A_n \in \A \implies A_1\cap A_2 \cap ... \cap A_n \in \A$$
Dizemos que $\A$ é uma álgebra de subconjuntos de $\o$.
Exemplos:
1) $\o = \{1,2,3\}$
$\A = \{A/A\subset\o\}$ é uma álgebra de subconjuntos.
$\A = \{\phi, \{1,2,3\}, \{1\}, \{2,3\}\}$  também é uma álgebra de subconjutnos de $\o$.
2) $\o = [0,1]$
$\A_1 = \{A|A\o\}$ é álgebra (mas não serve por incluir subconjuntos aos quais não é possível atribuir probabilidade).
$\A_2 = \{$ intervalos de $[0,1]\}$ não é álgebra.
$$A = [0,1/4) \in \A \mbox{ e } B = [3/4,1] \in \A \mbox{ mas } [0,1/4) \cup [3/4,1] \notin \A$$
$\A_3 = \{$ uniões finitas de intervalos possivelmente degenerados em $[0,1]\}$ é álgebra e é a menor álgebra que contém $\A_2$.

Definição: uma coleção $\A$ de subconjuntos de $\o$ é uma sigma álgebra de subconjuntos de $\o$ quando satisfaz 
1) $\o\in \A$
2) $A\in\A \implies A^c \in A$
3) $A_1,...,A_n \in \A \implies A_1\cup A_2 \cup ... \cup A_n \in \A = \cup_{n=1}^{\infty}A_n \in \A$
Toda $\sigma$-álgebra é uma álgebra.
Exemplo:$\o = \{1,2,3\}$
$\A \mbox{ é } \sigma$- álgebra se,  e somente se $\A$ é álgebra.
Exemplo: $\o=[0,1]$ 
$\mathbb{B}$ é álgebra de Borel.
$\mathbb{B}$ é a menor $\sigma$-álgebra que contém todos os intervalos
$\mathbb{B} = \cap\{\mathbb{F}|\mathbb{F}$ é sigma álgebra e $\mathbb{F}$ possui como elemento os intervalos$\}$
> $2^{\o}$ representa união de todos os conjuntos 

$\mathbb{F}_1\cap \mathbb{F}_2$ é sigma álgebra. 
Definição: um espaço de probabilidade é uma tripla $(\o,\A,P)$ onde 
- $\o$ é um conjunto (espaço amostral);
- $\A$ é sigma álgebra de subconjuntos de $\o$ (o conjunto dos eventos aleatórios).
- P é uma função de $\A$ em $\mathbb{R}$.
tal que:
1) $P(A)\geq0\forall A\in\A$
2) $P(\o) =1$
3) Se $A_1,A_2,... \in \A$ e são disjuntos 2 a 2, então $P(\cup_{n=1}^{\infty}A_n) = \sum_{n=1}^{\infty}P(A_n)$
Em particular se $A$ e $B$ são disjuntos, então $P(A\cup B) = P(A\cup B \cup \phi ...) = P(A)+P(B)+0+... = P(A)+P(B)$
Consequências:
1) $P(A^c)  = 1-P(A)$
$P(A^c\cup A) = 1$
2) $0\leq P(A) \leq 1$
3) $A\subset B \implies P(A)\leq P(B)$
4) $P(\cup_{i=1}^{n}A_i) \leq \sum_{i=1}^{n}P(A_i)$
5) $P(\cup_{i=1}^{\infty}A_i) \leq \sum_{i=1}^{\infty}P(A_n)$
6) Se $A_n \uparrow A$ então $P(A_n)\uparrow P(A)$. 
Se $A_n \downarrow A$ então $P(A_n)\downarrow P(A)$. 
Dizemos que $A_n \uparrow A$ quando $\forall n, A_n \subset A_{n+1}$ e $\cup_{n=1}^{\infty}A_n = A$ 
Exemplo:
$A_n = [0,1-1/n]$, então $A_n \uparrow [0,1)$

