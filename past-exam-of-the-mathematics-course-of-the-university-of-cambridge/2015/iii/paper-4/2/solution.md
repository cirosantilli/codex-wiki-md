<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

For central $t_1,\ldots,t_n$, define the [Koszul complex on central ring elements](../../../../../koszul-complex-on-central-ring-elements.md) using formal exterior symbols:

$$
K_k=\bigoplus_{1\leq i_1<\cdots<i_k\leq n}R\,e_{i_1}\wedge\cdots\wedge e_{i_k},\qquad K_0=R,
$$

with zero terms outside $0\leq k\leq n$ and differential

$$
d(r e_{i_1}\wedge\cdots\wedge e_{i_k})=\sum_{a=1}^k(-1)^{a-1}r t_{i_a}\,e_{i_1}\wedge\cdots\wedge\widehat{e_{i_a}}\wedge\cdots\wedge e_{i_k}.
$$

The terms are free [bimodules](../../../../../bimodule.md) with the formal symbols commuting with coefficients. Centrality makes $d$ a bimodule map, and the terms in $d^2$ cancel in pairs because the $t_i$ commute. This defines the [Koszul complex](../../../../../koszul-complex.md) over a possibly noncommutative ring without using an undefined exterior algebra of arbitrary one-sided modules. In particular $K(\mathbf t)\otimes_R M$ is a well-defined [chain complex](../../../../../chain-complex.md) of left modules.

A [regular sequence on a module](../../../../../regular-sequence-on-a-module.md) means that multiplication by $t_i$ is injective on $M/(t_1,\ldots,t_{i-1})M$ for each $i$, usually with the additional convention that the final quotient is nonzero. The homology vanishing below uses only the injectivity conditions. For one element, the [chain complex](../../../../../chain-complex.md) is $M\xrightarrow{t_1}M$, with zero first homology and zeroth homology $M/t_1M$.

For the induction let $C=K(t_1,\ldots,t_{n-1})\otimes_R M$. Adjoining the last generator identifies the new [Koszul complex](../../../../../koszul-complex.md) with the [mapping cone](../../../../../mapping-cone-homological-algebra.md) of multiplication by $t_n$ on $C$. In the convention $\operatorname{Cone}(t_n)_k=C_k\oplus C_{k-1}$ its differential is $(a,b)\mapsto(da+t_nb,-db)$; the identification is $a+e_n\wedge b$. The [long exact sequence in homology](../../../../../long-exact-sequence-in-homology.md) of this [mapping cone](../../../../../mapping-cone-homological-algebra.md) gives

$$
\cdots\longrightarrow H_k(C)\xrightarrow{t_n}H_k(C)\longrightarrow H_k(\operatorname{Cone}(t_n))\longrightarrow H_{k-1}(C)\xrightarrow{t_n}H_{k-1}(C)\longrightarrow\cdots.
$$

The induction hypothesis is $H_k(C)=0$ for $k>0$ and $H_0(C)=N=M/(t_1,\ldots,t_{n-1})M$. Regularity makes $t_n:N\to N$ injective. Hence the new positive homology is zero and its zeroth homology is $N/t_nN$. The augmentation to this quotient induces these homology isomorphisms, giving **the quasi-isomorphism**

$$
\boxed{K(\mathbf t)\otimes_R M\simeq M/(t_1,\ldots,t_n)M,}
$$

where the right side is placed in degree zero. The results used are the [long exact sequence in homology](../../../../../long-exact-sequence-in-homology.md) of a degreewise short exact sequence of complexes and its [mapping cone](../../../../../mapping-cone-homological-algebra.md) form, together with the stated induction; no unmentioned acyclicity criterion is needed.

For $R=\mathbb Z[X]$, $(p,X)$ is a [regular sequence](../../../../../regular-sequence.md): $p$ is a non-zero-divisor in $R$, and multiplication by $X$ is injective in $(\mathbb Z/p\mathbb Z)[X]$, even when $p$ is composite. The [Koszul resolution](../../../../../koszul-resolution.md) of $R/(p,X)$ is

$$
0\longrightarrow R\xrightarrow{\binom{-X}{p}}R^2\xrightarrow{(p\ \ X)}R\longrightarrow\mathbb Z/p\mathbb Z\longrightarrow0.
$$

With $N=\mathbb Z/q\mathbb Z$ and $X$ acting as zero, applying the [Hom functor](../../../../../hom-functor.md) gives the [cochain complex](../../../../../cochain-complex.md)

$$
N\xrightarrow{n\mapsto(pn,0)}N^2\xrightarrow{(u,v)\mapsto pv}N.
$$

Thus, more generally, the [Ext groups between polynomial-ring residue modules](../../../../../ext-groups-between-polynomial-ring-residue-modules.md) are

$$
\operatorname{Ext}_R^0=\ker(p:N\to N),\quad\operatorname{Ext}_R^1=(N/pN)\oplus\ker(p:N\to N),\quad\operatorname{Ext}_R^2=N/pN,
$$

and vanish in all degrees above two. **For the equal-modulus case**,

$$
\boxed{\operatorname{Ext}_{\mathbb Z[X]}^k(\mathbb Z/p\mathbb Z,\mathbb Z/p\mathbb Z)\cong\begin{cases}\mathbb Z/p\mathbb Z&k=0,2,\\(\mathbb Z/p\mathbb Z)^2&k=1,\\0&k>2.\end{cases}}
$$

These are $R$-modules through $X=0$ and reduction modulo $p$. If the multiplicative self-[Ext functor](../../../../../ext-functor.md) is desired, the [Koszul self-Ext algebra](../../../../../koszul-self-ext-algebra.md) is the exterior algebra on two degree-one generators over $\mathbb Z/p\mathbb Z$. The two contractions on the [Koszul resolution](../../../../../koszul-resolution.md) lift these classes, square to zero and anticommute, so this description also holds for composite $p$ and characteristic two. **For coprime $p,q$**, multiplication by $p$ is invertible on $N$, so both its kernel and cokernel vanish:

$$
\boxed{\operatorname{Ext}_{\mathbb Z[X]}^k(\mathbb Z/p\mathbb Z,\mathbb Z/q\mathbb Z)=0\quad\text{for every }k\geq0.}
$$

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 4](../../paper-4-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
