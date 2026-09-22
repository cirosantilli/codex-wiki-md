<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Write $k=\overline{\mathbb F}_q$, and let $F_0$ be the entrywise $q$th-power [Frobenius endomorphism of an algebraic group](../../../../../frobenius-endomorphism-of-an-algebraic-group.md) on the [general linear group](../../../../../general-linear-group.md) $G=\mathrm{GL}_2(k)$. The [algebraic closure](../../../../../algebraic-closure.md) is visible in the original PDF; it is lost in the converted TeX. Let $T_0$ be the diagonal [maximal algebraic torus](../../../../../maximal-algebraic-torus.md) and $B_0$ the upper triangular [Borel subgroup](../../../../../borel-subgroup.md).

Choose $\beta\in k$ with $\beta-\beta^q=1$. Such a $\beta$ exists because $k$ is an [algebraic closure](../../../../../algebraic-closure.md), and $\beta\notin\mathbb F_q$. Put

$$
h_+=\begin{pmatrix}1&\beta\\0&1\end{pmatrix},\qquad h_-=\begin{pmatrix}1&0\\\beta&1\end{pmatrix},\qquad F_\pm=\operatorname{Int}(h_\pm)\circ F_0\circ\operatorname{Int}(h_\pm)^{-1}.
$$

Transporting the standard $\mathbb F_q$-model through the [algebraic group](../../../../../algebraic-group.md) automorphism $\operatorname{Int}(h_\pm)$ gives a [rational structure on an algebraic group](../../../../../rational-structure-on-an-algebraic-group.md) over the same field $\mathbb F_q$. In particular these are genuine [Frobenius endomorphisms of an algebraic group](../../../../../frobenius-endomorphism-of-an-algebraic-group.md), and their fixed-point groups are

$$
G^{F_\pm}=h_\pm\mathrm{GL}_2(\mathbb F_q)h_\pm^{-1}.
$$

The auxiliary $\beta$ need not be rational for the original structure: it changes the identification with the geometric group, not the field over which the transported model is defined.

For either sign, take the [rational maximal torus](../../../../../rational-maximal-torus.md) and [Borel subgroup](../../../../../borel-subgroup.md)

$$
\boxed{T_\pm=h_\pm T_0h_\pm^{-1}\ \subset\ B_\pm=h_\pm B_0h_\pm^{-1}.}
$$

Indeed $F_\pm(h_\pm Hh_\pm^{-1})=h_\pm F_0(H)h_\pm^{-1}$ for $H=T_0,B_0$, so both subgroups are $F_\pm$-stable. Conjugacy also preserves maximality of the [algebraic torus](../../../../../algebraic-torus.md) and the property of being a [Borel subgroup](../../../../../borel-subgroup.md).

Finally,

$$
F_\pm=\operatorname{Int}(c_\pm)F_0,\qquad c_+=\begin{pmatrix}1&1\\0&1\end{pmatrix},\quad c_-=\begin{pmatrix}1&0\\1&1\end{pmatrix}.
$$

Neither $c_+$ nor $c_-$ is central, so neither endomorphism is $F_0$. If $F_+=F_-$, surjectivity of $F_0$ on $G(k)$ would imply that $c_-^{-1}c_+$ is central. But

$$
c_-^{-1}c_+=\begin{pmatrix}1&1\\-1&0\end{pmatrix}
$$

is not scalar in any characteristic. Thus **the two nonstandard rational structures have distinct Frobenius endomorphisms**, including when $q=2$.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 6](../../paper-6-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
