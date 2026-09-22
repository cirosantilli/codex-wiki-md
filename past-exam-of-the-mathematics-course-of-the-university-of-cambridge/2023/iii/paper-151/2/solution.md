<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

For the [free presentation](../../../../../free-presentation.md) $G=F/R$, conjugation in $F$ gives the [relation module](../../../../../relation-module.md)

$$
R_{\mathrm{ab}}=R/[R,R],
\qquad g\cdot(r[R,R])=frf^{-1}[R,R],
$$

where $f\in F$ is any lift of $g\in G$. A different lift differs by an element of $R$, whose inner conjugation acts trivially on the abelianization, so this is a well-defined $\mathbb ZG$-module action.

Choose free generators $x_1,\ldots,x_n$ of $F$. The [presentation relation sequence](../../../../../presentation-relation-sequence.md) becomes

$$
0\longrightarrow R_{\mathrm{ab}}
\xrightarrow{j}(\mathbb ZG)^n
\xrightarrow{d_1}\mathbb ZG
\xrightarrow{\varepsilon}\mathbb Z
\longrightarrow0,
$$

where $d_1(e_i)=\bar x_i-1$. In [Fox calculus](../../../../../fox-calculus.md), the first map is

$$
j(r[R,R])=
\sum_{i=1}^n\overline{\frac{\partial r}{\partial x_i}}e_i.
$$

The Fox identity $r-1=\sum_i(\partial r/\partial x_i)(x_i-1)$ gives $d_1j=0$, and the standard lifting argument in the free group proves exactness.

Split the sequence at the augmentation ideal $I_G$. Applying $\operatorname{Hom}_{\mathbb ZG}(-,M)$ to

$$
0\longrightarrow R_{\mathrm{ab}}\longrightarrow(\mathbb ZG)^n\longrightarrow I_G\longrightarrow0
$$

and using projectivity of $(\mathbb ZG)^n$ gives

$$
M^n\longrightarrow\operatorname{Hom}_G(R_{\mathrm{ab}},M)
\longrightarrow\operatorname{Ext}^1_{\mathbb ZG}(I_G,M)\longrightarrow0.
$$

The other short exact sequence $0\to I_G\to\mathbb ZG\to\mathbb Z\to0$ identifies the last group with $H^2(G,M)$. A [one-cocycle](../../../../../one-cocycle.md) on $F$ is a derivation and is determined freely by its values on $x_1,\ldots,x_n$, so $H^1(F,M)$ is $M^n$ modulo principal derivations. Principal derivations vanish on $R$, and restriction sends a derivation $d$ to the $G$-map $r[R,R]\mapsto d(r)$. The preceding cokernel sequence therefore descends to the [Mac Lane exact sequence for a free presentation](../../../../../mac-lane-exact-sequence-for-a-free-presentation.md)

$$
H^1(F,M)\longrightarrow\operatorname{Hom}_G(R_{\mathrm{ab}},M)
\longrightarrow H^2(G,M)\longrightarrow0.
$$

The left map need not be injective. Take $F=\langle t\rangle\cong\mathbb Z$, $R=\langle t^m\rangle$, $G\cong C_m$, and the trivial module $M=\mathbb Z/m\mathbb Z$, where $m>1$. Then $H^1(F,M)\cong M$, while restriction sends the derivation determined by $d(t)=a$ to

$$
d(t^m)=ma=0.
$$

**Thus the left map is zero although its domain is nonzero, and $R$ is nontrivial.**

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 151](../../paper-151-split.md)
3. [Iii](../../split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
