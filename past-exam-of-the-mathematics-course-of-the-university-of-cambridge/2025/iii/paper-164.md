# Paper 164

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2025/III_Paper_164.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2025/III_Paper_164.pdf)

**Table of contents**

- [1](#1)
  - [i](#1/i)
    - [Solution](#1/i/solution)
  - [ii](#1/ii)
    - [Solution](#1/ii/solution)
  - [iii](#1/iii)
    - [Solution](#1/iii/solution)
  - [iv](#1/iv)
    - [Solution](#1/iv/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [i](#3/i)
    - [Solution](#3/i/solution)
  - [ii](#3/ii)
    - [Solution](#3/ii/solution)
- [4](#4)
  - [i](#4/i)
    - [Solution](#4/i/solution)
  - [ii](#4/ii)
    - [Solution](#4/ii/solution)

## 1

↑ **Parent:** [Paper 164](paper-164.md)

<h3 id="1/i">i</h3>

↑ **Parent:** [1](#1)

<h4 id="1/i/solution">Solution</h4>

↑ **Parent:** [I](#1/i)

The axioms for [information entropy](../../../information-theory.md#information-entropy) give the formula $H(X)=-\sum_xp(x)\log p(x)$ and hence the [chain rule for information entropy](../../../information-theory.md#chain-rule-for-information-entropy)

$$
H(X,Y)=H(X)+H(Y\mid X).
$$

Because [conditioning reduces entropy](../../../information-theory.md#conditioning-reduces-entropy), $H(Y\mid X)\leq H(Y)$, and therefore

$$
H(X,Y)\leq H(X)+H(Y).
$$

This is [subadditivity of information entropy](../../../information-theory.md#subadditivity-of-information-entropy).

For the [entropy submodularity](../../../information-theory.md#entropy-submodularity) rule, apply the [chain rule for information entropy](../../../information-theory.md#chain-rule-for-information-entropy) twice:

$$
\begin{aligned}
H(X,Y)+H(Y,Z)-H(Y)-H(X,Y,Z)
&=H(X\mid Y)-H(X\mid Y,Z)\\
&=I(X;Z\mid Y)\geq0.
\end{aligned}
$$

The last quantity is [conditional mutual information](../../../information-theory.md#conditional-mutual-information), whose nonnegativity again expresses that [conditioning reduces entropy](../../../information-theory.md#conditioning-reduces-entropy).

<h3 id="1/ii">ii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1/ii)

Write $S_1=H(X)+H(Y)+H(Z)$ and $S_2=H(X,Y)+H(Y,Z)+H(Z,X)$. By the definition of [mutual information](../../../information-theory.md#mutual-information),

$$
I(X;Y)+I(Y;Z)+I(Z;X)=2S_1-S_2,
$$

so the required right-hand side is $(2S_2-S_1)/3$.

Apply [entropy submodularity](../../../information-theory.md#entropy-submodularity) to the pairs $(X,Y),(X,Z)$ and then cyclically permute the variables:

$$
\begin{aligned}
H(X,Y)+H(X,Z)&\geq H(X)+H(X,Y,Z),\\
H(Y,Z)+H(Y,X)&\geq H(Y)+H(X,Y,Z),\\
H(Z,X)+H(Z,Y)&\geq H(Z)+H(X,Y,Z).
\end{aligned}
$$

Adding gives $2S_2\geq S_1+3H(X,Y,Z)$, which is exactly

$$
\boxed{H(X,Y,Z)\leq\frac12S_2-\frac16(2S_1-S_2).}
$$

<h3 id="1/iii">iii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#1/iii)

Because $X,Y,Z$ are [independent random variables](../../../random-variable.md#independent-random-variables), adding $Y$ is an independent noise channel, so

$$
X\longrightarrow X+Z\longrightarrow X+Y+Z
$$

is a [Markov chain](../../../markov-process.md#markov-chain). The [data processing inequality for mutual information](../../../information-theory.md#data-processing-inequality) gives

$$
I(X;X+Y+Z)\leq I(X;X+Z).
$$

Translation in the [finite additive group](../../../group.md#finite-additive-group) preserves [conditional entropy](../../../information-theory.md#conditional-entropy), and independence therefore gives

$$
I(X;X+Y+Z)=H(X+Y+Z)-H(Y+Z)
$$

and

$$
I(X;X+Z)=H(X+Z)-H(Z).
$$

Substitution proves the required [entropy submodularity for three independent sums](../../../information-theory.md#entropy-submodularity-for-three-independent-sums).

<h3 id="1/iv">iv</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#1/iv)

For random variables $A,B$ in a [finite additive group](../../../group.md#finite-additive-group), take independent copies $A',B'$ with the same respective distributions and define the [Entropic Ruzsa distance](../../../information-theory.md#entropic-ruzsa-distance) by

$$
d_R(A,B)=H(A'-B')-\frac12H(A')-\frac12H(B').
$$

For the independent variables in the question, expansion gives

$$
d_R(X,Z)+d_R(Y,Z)-d_R(X,Y)
=H(X-Z)+H(Y-Z)-H(X-Y)-H(Z).
$$

Part iii, applied to the independent variables $X,Y,-Z$, says

$$
H(X+Y-Z)+H(Z)\leq H(X-Z)+H(Y-Z).
$$

Subtracting $H(X-Y)$ from both sides proves

$$
H(X+Y-Z)-H(X-Y)
\leq d_R(X,Z)+d_R(Y,Z)-d_R(X,Y).
$$

## 2

↑ **Parent:** [Paper 164](paper-164.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

Write $r=|V_0|$, $s=|V_1|$, and $e=|E(G)|=\alpha|X||Y|$. We construct a random [graph homomorphism](../../../graph-theory.md#graph-homomorphism) $\Psi:T\to G$. Choose a root of the [tree](../../../combinatorics.md#tree-graph-theory). Map it according to the [degree-biased vertex distribution](../../../graph-theory.md#degree-biased-vertex-distribution) on the corresponding side of the [bipartite graph](../../../graph-theory.md#bipartite-graph); after mapping any vertex, map each child independently and uniformly to a neighbour of its parent's image.

Every oriented tree edge is then mapped uniformly onto the $e$ edges of $G$. Every tree vertex in $V_0$ has the degree-biased marginal on $X$, of entropy $H_X$, and every vertex in $V_1$ has the analogous marginal of entropy $H_Y$. Repeated use of the [chain rule for information entropy](../../../information-theory.md#chain-rule-for-information-entropy) along the rooted tree gives

$$
H(\Psi)
=(k-1)\log e
-\sum_{v\in V_0}(\deg_Tv-1)H_X
-\sum_{v\in V_1}(\deg_Tv-1)H_Y.
$$

Since a $k$-vertex [tree](../../../combinatorics.md#tree-graph-theory) has $k-1$ edges,

$$
\sum_{v\in V_0}(\deg_Tv-1)=s-1,
\qquad
\sum_{v\in V_1}(\deg_Tv-1)=r-1.
$$

The [maximum entropy distribution on a finite set](../../../information-theory.md#maximum-entropy-distribution-on-a-finite-set) gives $H_X\leq\log|X|$ and $H_Y\leq\log|Y|$. Hence

$$
\begin{aligned}
H(\Psi)
&\geq(k-1)\log(\alpha|X||Y|)
-(s-1)\log|X|-(r-1)\log|Y|\\
&=\log\!\left(\alpha^{k-1}|X|^r|Y|^s\right).
\end{aligned}
$$

If $N$ is the number of bipartition-respecting [graph homomorphisms](../../../graph-theory.md#graph-homomorphism) $T\to G$, the support of $\Psi$ has size $N$, so the [maximum entropy distribution on a finite set](../../../information-theory.md#maximum-entropy-distribution-on-a-finite-set) also gives $H(\Psi)\leq\log N$. Thus

$$
N\geq\alpha^{k-1}|X|^r|Y|^s.
$$

There are $|X|^r|Y|^s$ bipartition-respecting maps in total, so a uniformly chosen one is a [graph homomorphism](../../../graph-theory.md#graph-homomorphism) with probability at least $\alpha^{k-1}$. This proves the [Sidorenko inequality for trees](../../../graph-theory.md#sidorenko-inequality-for-trees).

## 3

↑ **Parent:** [Paper 164](paper-164.md)

<h3 id="3/i">i</h3>

↑ **Parent:** [3](#3)

<h4 id="3/i/solution">Solution</h4>

↑ **Parent:** [I](#3/i)

Let

$$
c=\frac{3-\sqrt5}{2}=1-\frac1\varphi,
$$

where $\varphi$ is the [golden ratio](../../../algebra.md#golden-ratio). If the [union-closed family](../../../extremal-set-theory.md#union-closed-family) consists of one nonempty set, any element of that set has frequency one, so assume its cardinality exceeds one. Choose independent uniform members $A,B$ and let $X,Y\in\{0,1\}^n$ be their [characteristic vectors of sets](../../../extremal-set-theory.md#characteristic-vector-of-a-set). Then $H(X)=H(Y)=\log|\mathcal A|>0$.

Suppose for a contradiction that every element has frequency $p_i<c$. Put $q_i=1-p_i>1/\varphi$, and let $Z=X\mathbin{\mathrm{OR}}Y$, the [characteristic vector of a set](../../../extremal-set-theory.md#characteristic-vector-of-a-set) of $A\cup B$. The [chain rule for information entropy](../../../information-theory.md#chain-rule-for-information-entropy) and [conditioning reduces entropy](../../../information-theory.md#conditioning-reduces-entropy) give

$$
H(Z)=\sum_iH(Z_i\mid Z_{<i})
\geq\sum_iH(Z_i\mid X_{<i},Y_{<i}),
$$

because $Z_{<i}$ is a [function](../../../function.md) of $(X_{<i},Y_{<i})$.

Fix the two prefixes and set

$$
x=\mathbb P(X_i=0\mid X_{<i}),
\qquad
y=\mathbb P(Y_i=0\mid Y_{<i}).
$$

The two conditioned bits are [independent random variables](../../../random-variable.md#independent-random-variables), and $Z_i=0$ exactly when both are zero. The supplied [binary entropy product inequality](../../../extremal-set-theory.md#binary-entropy-product-inequality) therefore gives

$$
H(Z_i\mid X_{<i},Y_{<i})
=h_2(xy)
\geq\frac\varphi2\bigl(xh_2(y)+yh_2(x)\bigr).
$$

Averaging over the independent prefixes yields

$$
\begin{aligned}
H(Z_i\mid X_{<i},Y_{<i})
&\geq\frac\varphi2\bigl(q_iH(Y_i\mid Y_{<i})+q_iH(X_i\mid X_{<i})\bigr)\\
&>\frac12\bigl(H(Y_i\mid Y_{<i})+H(X_i\mid X_{<i})\bigr)
\end{aligned}
$$

whenever either conditional entropy is positive. Summing and using $H(X)>0$ gives $H(Z)>H(X)$.

But [set union](../../../set.md#set-union) keeps $A\cup B$ inside the [union-closed family](../../../extremal-set-theory.md#union-closed-family), so $Z$ is supported on $\mathcal A$. The [maximum entropy distribution on a finite set](../../../information-theory.md#maximum-entropy-distribution-on-a-finite-set) gives $H(Z)\leq\log|\mathcal A|=H(X)$, a contradiction. Some element must therefore occur in at least $c|\mathcal A|$ members, proving the [entropy bound for a union-closed family](../../../extremal-set-theory.md#entropy-bound-for-a-union-closed-family).

<h3 id="3/ii">ii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3/ii)

Let $\mathcal Q$ be the set of valid quintuples and choose $(A_1,\ldots,A_5)$ uniformly from $\mathcal Q$. Then

$$
H(A_1,\ldots,A_5)=\log|\mathcal Q|.
$$

Apply [Shearer's inequality](../../../information-theory.md#shearer-s-inequality) to the ten pairs $\{i,j\}\subseteq[5]$. Every index occurs in four pairs, so

$$
4H(A_1,\ldots,A_5)\leq\sum_{1\leq i<j\leq5}H(A_i,A_j).
$$

Put $U_{ij}=A_i\cup A_j$. Since $U_{ij}\in\mathcal A$, it has cardinality $k$. For each element of $U_{ij}$, its membership bits in $(A_i,A_j)$ are one of $(1,0),(0,1),(1,1)$; outside $U_{ij}$ they are forced to be $(0,0)$. Thus at most $3^k$ ordered pairs have any prescribed union. The [chain rule for information entropy](../../../information-theory.md#chain-rule-for-information-entropy), [conditional entropy](../../../information-theory.md#conditional-entropy), and the support bound for [information entropy](../../../information-theory.md#information-entropy) give

$$
H(A_i,A_j)
\leq H(U_{ij})+H(A_i,A_j\mid U_{ij})
\leq\log|\mathcal A|+k\log3,
$$

because every $U_{ij}$ belongs to $\mathcal A$. There are ten pairs, hence

$$
\log|\mathcal Q|
\leq\frac{10}{4}\bigl(\log|\mathcal A|+k\log3\bigr).
$$

Exponentiating proves

$$
|\mathcal Q|\leq3^{5k/2}|\mathcal A|^{5/2},
$$

which is the five-variable case of the [entropy bound for pairwise-union tuples](../../../extremal-set-theory.md#entropy-bound-for-pairwise-union-tuples).

## 4

↑ **Parent:** [Paper 164](paper-164.md)

<h3 id="4/i">i</h3>

↑ **Parent:** [4](#4)

<h4 id="4/i/solution">Solution</h4>

↑ **Parent:** [I](#4/i)

The [Entropic Balog-Szemerédi-Gowers theorem](../../../information-theory.md#entropic-balog-szemeredi-gowers-theorem) states that for finitely supported random variables $A,B$ in an [abelian group](../../../group.md#abelian-group),

$$
d_R(A;B\mathbin\Vert A+B)
\leq3I(A;B)+2H(A+B)-H(A)-H(B),
$$

where the left-hand side is the [Simultaneous conditional entropic Ruzsa distance](../../../information-theory.md#simultaneous-conditional-entropic-ruzsa-distance).

Put $S=A+B$ and take two copies $(A_1,B_1)$ and $(A_2,B_2)$ that are conditionally independent given $S$. Thus both sums equal $S$, and, given $S$, $A_1$ and $B_2$ are independent with the required conditional marginals. By [conditioning reduces entropy](../../../information-theory.md#conditioning-reduces-entropy),

$$
d_R(A;B\mathbin\Vert S)
\leq H(A_1-B_2)
-\frac12H(A_1\mid S)-\frac12H(B_2\mid S).
$$

The two conditional entropies are equal, since either $A$ or $B$ together with $S$ determines the other, and the [chain rule for information entropy](../../../information-theory.md#chain-rule-for-information-entropy) gives

$$
H(A\mid S)=H(B\mid S)
=H(A)+H(B)-I(A;B)-H(S).
$$

Set $D=A_1-B_2$. By [entropy submodularity](../../../information-theory.md#entropy-submodularity),

$$
H(D)\leq H(D,A_1)+H(D,B_1)-H(D,A_1,B_1).
$$

The first term is $H(A_1,B_2)\leq H(A)+H(B)$ by [subadditivity of information entropy](../../../information-theory.md#subadditivity-of-information-entropy). Since $A_1+B_1=A_2+B_2$, we also have $D=A_2-B_1$, so the second term is at most $H(A)+H(B)$. Finally $(D,A_1,B_1)$ determines all four copied variables, and conditional independence gives

$$
\begin{aligned}
H(D,A_1,B_1)
&=H(A_1,B_1,A_2,B_2)\\
&=H(S)+2H(A,B\mid S)\\
&=2H(A,B)-H(S).
\end{aligned}
$$

As $H(A,B)=H(A)+H(B)-I(A;B)$, these estimates imply

$$
H(D)\leq H(S)+2I(A;B).
$$

Subtracting the common conditional-entropy term proves the stated [Entropic Balog-Szemerédi-Gowers theorem](../../../information-theory.md#entropic-balog-szemeredi-gowers-theorem).

<h3 id="4/ii">ii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#4/ii)

Write $\delta=d_R(X,Y)$, $A=U_1+U_2$, $B=V_1+V_2$, and $S=A+B$. Distances depend only on distributions, so all variables used in any one application may be realized as [independent random variables](../../../random-variable.md#independent-random-variables).

First, the [entropy submodularity for three independent sums](../../../information-theory.md#entropy-submodularity-for-three-independent-sums) implies

$$
d_R(U_1+U_2,X)
\leq\frac12\bigl(2d_R(U,X)+d_R(U,U)\bigr),
$$

and analogously for $V$. The [Entropic Ruzsa triangle inequality](../../../information-theory.md#entropic-ruzsa-triangle-inequality) gives $d_R(U,U)\leq2d_R(U,X)$ and $d_R(V,V)\leq2d_R(V,Y)$. Consequently the [relevance of independent self-sums](../../../information-theory.md#relevance-of-independent-self-sums) gives

$$
p+q:=d_R(A,X)+d_R(B,Y)\leq2C\delta.
$$

Apply the [Conditioned entropic Ruzsa distance of a summand](../../../information-theory.md#conditioned-entropic-ruzsa-distance-of-a-summand) first to $(A,B,X)$ and then to $(B,A,Y)$:

$$
\begin{aligned}
d_R(A\mid S;X)&\leq\frac12\bigl(d_R(A,X)+d_R(B,X)+d_R(A,B)\bigr),\\
d_R(B\mid S;Y)&\leq\frac12\bigl(d_R(B,Y)+d_R(A,Y)+d_R(A,B)\bigr).
\end{aligned}
$$

Three applications of the [Entropic Ruzsa triangle inequality](../../../information-theory.md#entropic-ruzsa-triangle-inequality) give

$$
d_R(B,X)\leq q+\delta,
\qquad
d_R(A,Y)\leq p+\delta,
\qquad
d_R(A,B)\leq p+\delta+q.
$$

Adding all these bounds yields

$$
\begin{aligned}
d_R(A\mid S;X)+d_R(B\mid S;Y)
&\leq2(p+q+\delta)\\
&\leq(4C+2)\delta.
\end{aligned}
$$

**Thus the required absolute constants may be taken as $a=4$ and $b=2$.**

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2025](../../2025.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
