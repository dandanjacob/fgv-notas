$\newcommand{\A}{\mathbb{A}}$
$\newcommand{\o}{\Omega}$
> Aula passada

- Espaço de probabilidade $(\o, \A, P)$
Propriedades:
6) Se $A_n \uparrow A$, então $P(A_n)\uparrow P(A)$
Aqui, $A_n \uparrow A$ significa que como $A_n \subset A_{n+1}, \forall n$, 
$$\cup_{n=1}^{\infty} = \{x \mbox{ tais que } \exists n \mbox{ tal que } x\in A_n $$
$$A_1 \cup A_2 \cup \dots $$
 Se $A_n \downarrow A$, então $P(A_n)\downarrow P(A)$
 Caso particular: Se $A_n \downarrow \phi$ então $P(A_n)\downarrow \phi$. (continuidade do vazio)
 Se $A_1,A_2, \dots$ são disjuntos 2 a 2, então 
 $$P(\cup_{n=1}^{\infty} = \sum_{n=1}^{\infty}P(A_n)$$
 Exemplo: 
 ![[Pasted image 20230314131041.png]]
 Seja $B_1 = A_1$
 Para cada $n>1$, seja $B_n = A_n - A_{n-1}$
 Então $\cup_{n=1}^{\infty}A_n = \cup_{n=1}^{\infty}B_n$ 
 Como $\cup_{n=1}^{\infty}B_n$ é uma união disjunta, temos 
 $$P(A) = P(\cup_{n=1}^{\infty}B_n) = \sum_{n=1}^{\infty}P(B_n) = \sum_{n=1}^{\infty}[P(A_n)-P(A_{n-1})] = \lim_{n \longmapsto \infty}P(A_n)$$
 > Verdadeiro ou falso?
 > Se $\cup_{n=1}^{\infty}A_n=A$, então $\lim_{n\longmapsto\infty}P(A_n) = P(A)$
 > Falso!
 > Os intervlos $A_n$ podem ser 
 > $A_1, \phi, A_2, \phi, \dots$

Como construir espaços de probabilidade?
a) Caso discreto: $\o = \{ w_1,w_2, \dots \}$
Definir $p_i = P(\{w_i\})$ para cada $i$, de modo que $\sum pi=1$
$\A = 2^{\o} = \{A|A\subset \o\}$
$\forall A \in \A$, definir $P(A) = \sum_{w_1 \in \A}p_i$
1) $P(A)\geq 0$
2) $P(\o) = \sum p_i = 1$
3) Se A e B são disjuntos
$$P(A\cup B) = \sum_{w_i \in A \cup B}p_i = \sum_{w_i \in A}p_i + \sum_{w_i \in  B}p_i = P(A) + P(B)$$
b) Caso contínuo: $\o = \r$ (ou um intervalo)
- $A=B(\sigma$-álgebra de Borel) (menor álgebra que contém todos os intervalos)
- Definir probabilidade para os intervalos e estender para a álgebra os intervalos de modo que valham as proprosições 1,2, e 3.
$$P(-\infty, a] \longmapsto P(x), x \in B$$
satisfazendo algumas condições

#### Definição 
A probabilidade condicional de A dado B  $(A,B \in \A e P(B)>0$ é:
$$P(A|B) = \frac{P(A\cap B)}{P(B)}$$
Obs: i) $P(B|B) = 1$
ii) $(\o, \A, P(.|B))$ é um novo espaço de probabilidade

Exemplo: Dado equilibrado lançado das vezes;
1) $A =$ 1º resultado sair 5
2) $B =$ soma=6
3) $C =$ soma=2
a) $P(A) = 1/6$
b) $P(B) = 1/5$
c) $P(C) = 0$

Exemplo: uma urna contém 6 bolas brancas e 4 bolas pretas tiradas uma a uma sem reposição 
Qual é a probbilidade de 
a) 1ª branca e 2ª preta?p