# Paper 160

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2021/paper_160.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2021/paper_160.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [i](#1/c/i)
      - [Solution](#1/c/i/solution)
    - [ii](#1/c/ii)
      - [Solution](#1/c/ii/solution)
    - [iii](#1/c/iii)
      - [Solution](#1/c/iii/solution)
- [2](#2)
  - [a](#2/a)
    - [i](#2/a/i)
      - [Solution](#2/a/i/solution)
    - [ii](#2/a/ii)
      - [Solution](#2/a/ii/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
  - [d](#2/d)
    - [i](#2/d/i)
      - [Solution](#2/d/i/solution)
    - [ii](#2/d/ii)
      - [Solution](#2/d/ii/solution)
- [3](#3)
  - [a](#3/a)
    - [i](#3/a/i)
      - [Solution](#3/a/i/solution)
    - [ii](#3/a/ii)
      - [Solution](#3/a/ii/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [i](#3/c/i)
      - [Solution](#3/c/i/solution)
    - [ii](#3/c/ii)
      - [Solution](#3/c/ii/solution)
    - [iii](#3/c/iii)
      - [Solution](#3/c/iii/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)

## 1

↑ **Parent:** [Paper 160](paper-160.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Expand the [Column antisymmetrizer of a Young tableau](../../../representation-theory-of-the-symmetric-group.md#column-antisymmetrizer-of-a-young-tableau):

$$
b_v\{w\}=\sum_{g\in C(v)}\operatorname{sgn}(g)\{gw\}.
$$

If two entries in one column of $v$ lie in the same row of $w$, their transposition belongs to both $C(v)$ and the row stabilizer of $w$, so the terms cancel in pairs. The assumption $b_v\{w\}\ne0$ therefore says that every row of $w$ meets every column of $v$ in at most one entry.

The first row of $w$ has $\lambda_1$ entries, while $v$ has exactly $\lambda_1$ nonempty columns. It must consequently contain exactly one entry from each column of $v$. Permuting within each column puts these entries in the first row positions of $v$. Delete the matched first rows and repeat the argument on the remaining [Young diagram](../../../representation-theory-of-the-symmetric-group.md#young-diagram). The product of the resulting column permutations is an element $h\in C(v)$ for which the row sets of $hv$ are those of $w$. Thus

$$
\boxed{h\{v\}=\{w\}}.
$$

This is the [nonzero column antisymmetrizer criterion](../../../representation-theory-of-the-symmetric-group.md#nonzero-column-antisymmetrizer-criterion).

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

The [James submodule theorem](../../../representation-theory-of-the-symmetric-group.md#james-submodule-theorem) says that for every $FS_n$-submodule $U\leq M^\lambda$, either

$$
S^\lambda\subseteq U
\qquad\text{or}\qquad
U\subseteq(S^\lambda)^\perp,
$$

where orthogonality is taken with respect to the [tabloid bilinear form](../../../representation-theory-of-the-symmetric-group.md#tabloid-bilinear-form).

Fix a $\lambda$-tableau $t$. Part a shows that for every tabloid $\{s\}$, the vector $b_t\{s\}$ is either zero or a signed copy of the [polytabloid](../../../representation-theory-of-the-symmetric-group.md#polytabloid) $e(t)$. Comparing the coefficient of $\{t\}$ gives the precise identity

$$
b_tu=\langle u,e(t)\rangle e(t)
\qquad (u\in M^\lambda).
$$

If $U\nsubseteq(S^\lambda)^\perp$, choose $u\in U$ and a tableau $t$ with $\langle u,e(t)\rangle\ne0$. Since $U$ is a submodule, the identity puts $e(t)$ in $U$. Every polytabloid of shape $\lambda$ is an $S_n$-translate of $e(t)$, so their span $S^\lambda$ lies in $U$. If no such $u,t$ exist, then by definition $U\subseteq(S^\lambda)^\perp$. This proves the theorem over the arbitrary field $F$.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/i">i</h4>

↑ **Parent:** [C](#1/c)

<h5 id="1/c/i/solution">Solution</h5>

↑ **Parent:** [I](#1/c/i)

The row stabilizer of the transposed tableau is $R(t')=C(t)$. For $r\in R(t')$, the [polytabloid](../../../representation-theory-of-the-symmetric-group.md#polytabloid) satisfies

$$
r e(t)=\operatorname{sgn}(r)e(t),
\qquad
r e(u)=\operatorname{sgn}(r)e(u).
$$

The two signs cancel in the tensor product, so

$$
gr e(t)\otimes gr e(u)=g e(t)\otimes g e(u).
$$

Thus the proposed value depends only on the tabloid $\{gt'\}$ and $\theta$ is well-defined. Its definition immediately gives

$$
\theta(k\{gt'\})=k\theta(\{gt'\}),
$$

so it is an $FS_n$-homomorphism. Since any $e(w)$ is $g e(t)$ for some $g$, its images contain every generator $e(w)\otimes e(u)$ of $S^\lambda\otimes S^{(1^n)}$. Hence $\theta$ is surjective.

<h4 id="1/c/ii">ii</h4>

↑ **Parent:** [C](#1/c)

<h5 id="1/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/c/ii)

Because $C(t')=R(t)$,

$$
e(t')=\sum_{r\in R(t)}\operatorname{sgn}(r)\{rt'\}.
$$

Applying $\theta$ and using $r e(u)=\operatorname{sgn}(r)e(u)$ gives

$$
\theta(e(t'))=\left(\sum_{r\in R(t)}r e(t)\right)\otimes e(u).
$$

Thus $m=\sum_{r\in R(t)}r e(t)$. Every $r$ fixes the tabloid $\{t\}$, while $e(t)$ has coefficient one at $\{t\}$. Invariance of the [tabloid bilinear form](../../../representation-theory-of-the-symmetric-group.md#tabloid-bilinear-form) now yields

$$
\langle m,\{t\}\rangle
=\sum_{r\in R(t)}\langle r e(t),\{t\}\rangle
=\sum_{r\in R(t)}1
=\boxed{|R(t)|}.
$$

<h4 id="1/c/iii">iii</h4>

↑ **Parent:** [C](#1/c)

<h5 id="1/c/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#1/c/iii)

The preceding part shows that $\theta(e(t'))\ne0$ in characteristic zero, so $S^{\lambda'}\nsubseteq\ker\theta$. Apply the [James submodule theorem](../../../representation-theory-of-the-symmetric-group.md#james-submodule-theorem) to the proper submodule $\ker\theta\leq M^{\lambda'}$ to obtain

$$
\ker\theta\subseteq(S^{\lambda'})^\perp.
$$

The [Hook-length formula](../../../representation-theory-of-the-symmetric-group.md#hook-length-formula) gives $\dim S^\lambda=\dim S^{\lambda'}$. Surjectivity of $\theta$ therefore gives

$$
\operatorname{codim}\ker\theta=\dim S^\lambda=\dim S^{\lambda'}
=\operatorname{codim}(S^{\lambda'})^\perp,
$$

and hence

$$
\boxed{\ker\theta=(S^{\lambda'})^\perp}.
$$

Fix the original tableaux $t,u$. For a $\lambda$-tableau $w$, let $g_w$ be the unique permutation satisfying $w=g_wt$ and put $\varepsilon_w=\operatorname{sgn}(g_w)$. Since

$$
\theta(\{w'\})=\varepsilon_w e(w)\otimes e(u),
$$

the quotient pairing $M^{\lambda'}/(S^{\lambda'})^\perp\cong(S^{\lambda'})^*$ gives the explicit [conjugate Specht module as a sign-twisted dual](../../../representation-theory-of-the-symmetric-group.md#conjugate-specht-module-as-a-sign-twisted-dual) isomorphism

$$
e(w)\otimes e(u)longmapsto
\left[e(v')\longmapsto
\varepsilon_w\langle\{w'\},e(v')\rangle\right]
$$

for every $\lambda$-tableau $w$.

## 2

↑ **Parent:** [Paper 160](paper-160.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/i">i</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/i/solution">Solution</h5>

↑ **Parent:** [I](#2/a/i)

Write $a=\lambda-\mathrm{id}$. The two modified entries satisfy

$$
\mu_i-i=\lambda_{i+1}-(i+1)=a_{i+1},
\qquad
\mu_{i+1}-(i+1)=\lambda_i-i=a_i.
$$

Thus $\mu-\mathrm{id}$ is obtained from $\lambda-\mathrm{id}$ by the adjacent transposition $\tau=(i,i+1)$. In the alternating definition of $\psi$, reindexing $\pi$ by $\tau\pi$ preserves every induced permutation character and reverses every sign. Therefore the [straightening of a symmetric-group character indexed by a composition](../../../representation-theory-of-the-symmetric-group.md#straightening-of-a-symmetric-group-character-indexed-by-a-composition) gives

$$
\boxed{\psi^\mu=-\psi^\lambda}.
$$

<h4 id="2/a/ii">ii</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/a/ii)

The restriction form of the [restriction branching rule for a symmetric group](../../../representation-theory-of-the-symmetric-group.md#restriction-branching-rule-for-a-symmetric-group) is

$$
\boxed{\operatorname{Res}^{S_n}_{S_{n-1}}S^\lambda
\cong\bigoplus_{\mu\in\lambda^-}S^\mu},
$$

where $\lambda^-$ contains the distinct partitions obtained by deleting one [Removable node of a Young diagram](../../../representation-theory-of-the-symmetric-group.md#removable-node-of-a-young-diagram). In particular, the restriction is multiplicity-free.

Restrict the alternating expression

$$
\psi^\lambda=\sum_{\pi\in S_N}\operatorname{sgn}(\pi)\xi^{\lambda-\mathrm{id}+\pi}.
$$

The supplied restriction formula for a Young permutation character, with $k=1$, says that each term restricts by subtracting one from each possible component. After collecting the alternating sums, this gives

$$
\operatorname{Res}^{S_n}_{S_{n-1}}\psi^\lambda
=\sum_i\psi^{\lambda-\epsilon_i}.
$$

If row $i$ has no removable node, part i straightens $\psi^{\lambda-\epsilon_i}$ against the adjacent term with the opposite sign, or makes it zero when two shifted entries coincide. The surviving terms are exactly $\psi^\mu$ for $\mu\in\lambda^-$. Since $\lambda$ and each surviving $\mu$ are partitions, $\psi^\lambda=\chi^\lambda$ and $\psi^\mu=\chi^\mu$. We obtain

$$
\operatorname{Res}^{S_n}_{S_{n-1}}\chi^\lambda
=\sum_{\mu\in\lambda^-}\chi^\mu.
$$

Complex representations of a [finite group](../../../group.md#finite-group) are semisimple, so equality of characters proves the asserted module decomposition.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Repeated use of the induction branching rule gives

$$
S^{(2)}\!\uparrow_{S_2}^{S_4}
\cong S^{(4)}\oplus2S^{(3,1)}\oplus S^{(2,2)}\oplus S^{(2,1,1)},
$$

while

$$
S^{(1^3)}\!\uparrow_{S_3}^{S_4}
\cong S^{(2,1,1)}\oplus S^{(1^4)}.
$$

On the five conjugacy classes $1,(12),(12)(34),(123),(1234)$, their characters are respectively

$$
(12,2,0,0,0)
\quad\text{and}\quad
(4,-2,0,1,0).
$$

The tensor-product character is their pointwise product $(48,-4,0,0,0)$. Taking [inner products](../../../representation-theory.md#character-orthogonality) with the five irreducible characters of $S_4$ gives multiplicities $1,5,4,7,3$. Therefore the [induced-tensor decomposition for the symmetric group on four points](../../../representation-theory-of-the-symmetric-group.md#induced-tensor-decomposition-for-the-symmetric-group-on-four-points) is

$$
\boxed{V\cong S^{(4)}\oplus5S^{(3,1)}\oplus4S^{(2,2)}\oplus7S^{(2,1,1)}\oplus3S^{(1^4)}}.
$$

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Use the [character formula for an induced representation](../../../representation-theory.md#character-formula-for-an-induced-representation). For $g\in G$,

$$
\begin{aligned}
\chi(g)(\phi\!\uparrow_H^G)(g)
&=\frac1{|H|}\sum_{\substack{x\in G\\x^{-1}gx\in H}}
\chi(g)\phi(x^{-1}gx)\\
&=\frac1{|H|}\sum_{\substack{x\in G\\x^{-1}gx\in H}}
\chi(x^{-1}gx)\phi(x^{-1}gx)\\
&=\bigl((\chi\!\downarrow_H)\phi\bigr)\!\uparrow_H^G(g).
\end{aligned}
$$

The middle equality uses that a [character of a representation](../../../representation-theory.md#character-of-a-representation) is constant on conjugacy classes. This proves the [tensor identity for an induced character](../../../representation-theory-of-the-symmetric-group.md#tensor-identity-for-an-induced-character).

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/i">i</h4>

↑ **Parent:** [D](#2/d)

<h5 id="2/d/i/solution">Solution</h5>

↑ **Parent:** [I](#2/d/i)

The point-permutation character is

$$
\xi^{(n-1,1)}=1\!\uparrow_{S_{n-1}}^{S_n}
=\chi^{(n)}+\chi^{(n-1,1)}.
$$

By the [tensor identity for an induced character](../../../representation-theory-of-the-symmetric-group.md#tensor-identity-for-an-induced-character) and [Frobenius reciprocity](../../../representation-theory.md#frobenius-reciprocity),

$$
\langle\chi^\lambda\chi^\lambda,\xi^{(n-1,1)}\rangle
=\left\langle
\chi^\lambda\!\downarrow_{S_{n-1}},
\chi^\lambda\!\downarrow_{S_{n-1}}
\right\rangle.
$$

The [restriction branching rule for a symmetric group](../../../representation-theory-of-the-symmetric-group.md#restriction-branching-rule-for-a-symmetric-group) is multiplicity-free with one constituent for each member of $\lambda^-$, so the right side is $|\lambda^-|$. Also $\langle\chi^\lambda\chi^\lambda,\chi^{(n)}\rangle=1$ because every symmetric-group character is real and irreducible. Subtracting the trivial constituent proves the [standard-character multiplicity in a Specht self-product](../../../representation-theory-of-the-symmetric-group.md#standard-character-multiplicity-in-a-specht-self-product) formula

$$
\boxed{\langle\chi^\lambda\chi^\lambda,\chi^{(n-1,1)}\rangle=|\lambda^-|-1}.
$$

<h4 id="2/d/ii">ii</h4>

↑ **Parent:** [D](#2/d)

<h5 id="2/d/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/d/ii)

Suppose $\chi^\alpha\chi^\beta$ is irreducible. Since symmetric-group characters are real,

$$
1=\langle\chi^\alpha\chi^\beta,\chi^\alpha\chi^\beta\rangle
=\langle\chi^\alpha\chi^\alpha,\chi^\beta\chi^\beta\rangle.
$$

Both self-products contain the trivial character once. They can therefore have no other common irreducible constituent. By part i, the standard character occurs in the two self-products with multiplicities $|\alpha^-|-1$ and $|\beta^-|-1$. Hence one of these numbers is zero; say $|\alpha^-|=1$.

A partition has exactly one removable node precisely when all its nonzero rows have equal length, so $\alpha=(a^b)$ is rectangular. Since $ab=n$ and $n$ is [prime](../../../number-theory.md#prime-number), either $a=1$ or $b=1$. Thus $\alpha=(1^n)$ or $(n)$. The same argument applies with $\alpha$ and $\beta$ interchanged, proving the [prime-degree irreducible Kronecker product criterion for a symmetric group](../../../representation-theory-of-the-symmetric-group.md#prime-degree-irreducible-kronecker-product-criterion-for-a-symmetric-group).

## 3

↑ **Parent:** [Paper 160](paper-160.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/i">i</h4>

↑ **Parent:** [A](#3/a)

<h5 id="3/a/i/solution">Solution</h5>

↑ **Parent:** [I](#3/a/i)

Trace the southeast boundary of the [hook of a Young diagram](../../../representation-theory-of-the-symmetric-group.md#hook-of-a-young-diagram) based at $(i,j)$. At each horizontal boundary step record the hook length $h_{i,y}$ of the cell in row $i$ above that step. At each vertical step ending beside row $x$, record $h_{i,j}-h_{x,j}$. Starting at the northeast end and moving to the southwest end, these records increase by one from $1$ to $h_{i,j}$; horizontal and vertical steps are disjoint and account for every step. Therefore the [Hook-interval decomposition at a Young-diagram cell](../../../representation-theory-of-the-symmetric-group.md#hook-interval-decomposition-at-a-young-diagram-cell) is

$$
\boxed{
\{1,\ldots,h_{i,j}\}
=\{h_{i,y}:j\leq y\leq\lambda_i\}
\sqcup
\{h_{i,j}-h_{x,j}:i<x\leq\lambda'_j\}.}
$$

<h4 id="3/a/ii">ii</h4>

↑ **Parent:** [A](#3/a)

<h5 id="3/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/a/ii)

The supplied row-hook formula is

$$
H_i(\lambda)=\{1,\ldots,h_i\}
\setminus\{h_i-h_j:i<j\leq m\}.
$$

Consequently $h\in H_i(\lambda)$ exactly when $h_i-h\geq0$ and $h_i-h$ is not one of $h_{i+1},\ldots,h_m$. Since $h_i-h\leq h_i<h_j$ for $j<i$, this is equivalent to $h_i-h\notin X$. We have proved the [hook criterion in a beta set](../../../representation-theory-of-the-symmetric-group.md#hook-criterion-in-a-beta-set)

$$
\boxed{h\in H_i(\lambda)\Longleftrightarrow h_i-h\geq0\text{ and }h_i-h\notin X}.
$$

If $ef$ is a hook length, the beta-set interpretation gives a bead at some position $b$ and a gap at $b-ef$. In the finite progression

$$
b,b-e,b-2e,\ldots,b-fe,
$$

the first position is occupied and the last is empty. Some consecutive pair is therefore a bead followed by a gap. Their distance is $e$, so the criterion gives a hook of length $e$. This proves the [divisor closure of hook lengths](../../../representation-theory-of-the-symmetric-group.md#divisor-closure-of-hook-lengths).

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Let

$$
D(\lambda)=\#\{\text{odd hook lengths of }\lambda\}
-\#\{\text{even hook lengths of }\lambda\}.
$$

A direct comparison of the affected bead-gap pairs shows that removing a rim 2-hook preserves $D$: the pairs whose parities change cancel in odd-even pairs. Repeating this removal gives

$$
D(\lambda)=D(C_2(\lambda)).
$$

Every [2-core](../../../representation-theory-of-the-symmetric-group.md#core-of-a-partition) is a staircase

$$
(r,r-1,\ldots,1).
$$

All hook lengths in this staircase are odd, and it has $1+2+\cdots+r=r(r+1)/2$ cells. Hence the [odd-minus-even hook count of a partition](../../../representation-theory-of-the-symmetric-group.md#odd-minus-even-hook-count-of-a-partition) is

$$
\boxed{D(\lambda)=\binom{r+1}{2}}.
$$

**Thus the requested integer is $m=r+1=\ell(C_2(\lambda))+1$.**

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/i">i</h4>

↑ **Parent:** [C](#3/c)

<h5 id="3/c/i/solution">Solution</h5>

↑ **Parent:** [I](#3/c/i)

Use four beads, for which $(3,1)$ has [beta set](../../../representation-theory-of-the-symmetric-group.md#beta-set-of-a-partition)

$$
\{6,3,1,0\}.
$$

On runners of residues $0,1,2,3$, division by four gives respectively the beta sets

$$
\{0\},\quad\{0\},\quad\{1\},\quad\{0\}.
$$

Only $\{1\}$ represents a nonempty partition, namely $(1)$. Therefore the [four-quotient of the partition three-one](../../../representation-theory-of-the-symmetric-group.md#four-quotient-of-the-partition-three-one) is

$$
\boxed{Q_4(3,1)=(\varnothing,\varnothing,(1),\varnothing)}.
$$

<h4 id="3/c/ii">ii</h4>

↑ **Parent:** [C](#3/c)

<h5 id="3/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/c/ii)

A two-runner [partition abacus](../../../representation-theory-of-the-symmetric-group.md#abacus-of-a-partition) gives

$$
Q_2(3,1)=((2),\varnothing),
\qquad
Q_2(2)=(\varnothing,(1)),
$$

and the 2-quotients of $(1)$ and $\varnothing$ are empty. Thus the [two-quotient tower of the partition three-one](../../../representation-theory-of-the-symmetric-group.md#two-quotient-tower-of-the-partition-three-one) has nonempty levels

$$
\boxed{
TQ_2(3,1)_0=((3,1)),
\quad TQ_2(3,1)_1=((2),\varnothing),
\quad TQ_2(3,1)_2=(\varnothing,(1),\varnothing,\varnothing).}
$$

<h4 id="3/c/iii">iii</h4>

↑ **Parent:** [C](#3/c)

<h5 id="3/c/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#3/c/iii)

An $e^k$-runner abacus separates bead positions by their residue modulo $e^k$. Write such a residue in base $e$ as

$$
a_0+a_1e+\cdots+a_{k-1}e^{k-1}.
$$

Taking one $e$-quotient sorts beads by $a_0$ and divides their positions by $e$; applying the operation again sorts by $a_1$, and so on. After $k$ stages, the iterated construction has selected exactly the same $e^k$ residue classes as the single $e^k$-quotient. The two conventional orderings may list the base-$e$ digits in opposite order, producing only a permutation of components.

Equivalently, induction on $k$ applies the same argument to every component of $Q_e(\lambda)$ and identifies the resulting $e^{k+1}$ runner partitions. Hence the [iterated quotient equals a power quotient up to permutation](../../../representation-theory-of-the-symmetric-group.md#iterated-quotient-equals-a-power-quotient-up-to-permutation) statement is

$$
\boxed{Q_{e^k}(\lambda)\text{ is a permutation of }TQ_e(\lambda)_k}.
$$

## 4

↑ **Parent:** [Paper 160](paper-160.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

Put

$$
q_r=|TQ_p(\lambda)_r|,
\qquad
c_r=|TC_p(\lambda)_r|.
$$

The defining relation between the [quotient tower of a partition](../../../representation-theory-of-the-symmetric-group.md#quotient-tower-of-a-partition) and the [core tower of a partition](../../../representation-theory-of-the-symmetric-group.md#core-tower-of-a-partition) is

$$
q_r=c_r+pq_{r+1},
\qquad q_0=n.
$$

Summing the resulting telescoping identities gives

$$
\sum_{r\geq0}c_r=n-(p-1)\sum_{r\geq1}q_r.
$$

By the [Hook-length formula](../../../representation-theory-of-the-symmetric-group.md#hook-length-formula),

$$
v_p(\chi^\lambda(1))=v_p(n!)-\sum_{x\in Y(\lambda)}v_p(h_x).
$$

The [abacus divisible-hook correspondence](../../../representation-theory-of-the-symmetric-group.md#hooks-divisible-by-the-abacus-modulus) says that the number of hooks divisible by $p^r$ is $q_r$, so

$$
\sum_xv_p(h_x)=\sum_{r\geq1}q_r.
$$

If $d_p(n)=\sum_r\alpha_r$, the digit-sum form of the [Legendre formula](../../../number-theory.md#legendre-s-formula) is

$$
v_p(n!)=\frac{n-d_p(n)}{p-1}.
$$

Combining the three displayed identities proves the [P-adic valuation of a symmetric-group character degree from the core tower](../../../representation-theory-of-the-symmetric-group.md#p-adic-valuation-of-a-symmetric-group-character-degree-from-the-core-tower) formula

$$
\boxed{
v_p(\chi^\lambda(1))
=\frac{\sum_{r\geq0}|TC_p(\lambda)_r|-\sum_{r\geq0}\alpha_r}{p-1}.}
$$

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Add the base-$p$ expansions of $x$ and $y$ column by column. Before carrying, the sum of all displayed digits is $d_p(x)+d_p(y)$. Each carry removes $p$ units from one column and adds one unit to the next, decreasing the total digit sum by $p-1$. After all carries the digits are those of $x+y$, so the [subadditivity of the base-p digit sum](../../../number-theory.md#subadditivity-of-the-base-p-digit-sum) gives

$$
\boxed{d_p(x+y)\leq d_p(x)+d_p(y)}.
$$

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

Let $\mu=C_p(\lambda)$, put $m=|\mu|$, and let the first-level $p$-quotient partitions have sizes $n_0,\ldots,n_{p-1}$. Then

$$
n=m+p\sum_jn_j.
$$

Repeated [subadditivity of the base-p digit sum](../../../number-theory.md#subadditivity-of-the-base-p-digit-sum) gives

$$
d_p(n)-d_p(m)
\leq d_p\left(\sum_jn_j\right)
\leq\sum_jd_p(n_j).
$$

For any partition $\nu$ of size $s$, iterating the core-quotient relation $s=|C_p(\nu)|+p|Q_p(\nu)|$ and the same digit-sum inequality gives

$$
d_p(s)\leq\sum_{r\geq0}|TC_p(\nu)_r|.
$$

Apply this to every first-level quotient partition. Their core towers concatenate to levels $r\geq1$ of $TC_p(\lambda)$, so

$$
d_p(n)-d_p(m)
\leq\sum_{r\geq1}|TC_p(\lambda)_r|.
$$

Part a applied to $\lambda$ and to its $p$-core $\mu$, whose higher core-tower levels are empty, now gives

$$
\begin{aligned}
(p-1)\left(v_p(\chi^\lambda(1))-v_p(\chi^\mu(1))\right)
&=\sum_{r\geq1}|TC_p(\lambda)_r|-d_p(n)+d_p(m)\\
&\geq0.
\end{aligned}
$$

Therefore the [Character-degree valuation does not increase on taking the p-core](../../../representation-theory-of-the-symmetric-group.md#character-degree-valuation-does-not-increase-on-taking-the-p-core):

$$
\boxed{v_p(\chi^\lambda(1))\geq v_p(\chi^{C_p(\lambda)}(1))}.
$$

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2021](../../2021.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
