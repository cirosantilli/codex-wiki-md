<h1 id="23g/solution">Solution</h1>

↑ **Parent:** [23G](../23g.md)

A functional $p:X\to\mathbb R$ is [sublinear](../../../../../sublinear-function.md) when

$$
p(u+v)\leq p(u)+p(v),\qquad p(tu)=tp(u)\quad(t\geq0).
$$

Any extension to $\widetilde M=M+\mathbb Rx$ must have the form

$$
\widetilde\ell(y+tx)=\ell(y)+tc.
$$

Choose $c$ satisfying

$$
\sup_{y\in M}\{\ell(y)-p(y-x)\}
\leq c\leq
\inf_{y\in M}\{p(y+x)-\ell(y)\}.
$$

This interval is nonempty: for $y,z\in M$,

$$
\ell(y)+\ell(z)=\ell(y+z)
\leq p(y+z)
\leq p(y-x)+p(z+x),
$$

which rearranges to the required lower bound being at most the upper bound. For $t>0$, positive homogeneity reduces  
$\widetilde\ell(y+tx)\leq p(y+tx)$ to the upper inequality after replacing $y$ by $y/t$; for $t<0$ it reduces to the lower inequality. The case $t=0$ is the hypothesis on $\ell$. Thus this choice gives the required dominated linear extension.

The dominated form of the [Hahn-Banach theorem](../../../../../hahn-banach-theorem.md) states that a linear functional on a subspace, bounded above by a sublinear functional, extends linearly to the whole real vector space while retaining that bound.

Let $M=\operatorname{span}\{z_1,\ldots,z_n\}$. Its coordinate maps

$$
\lambda_j\!\left(\sum_ka_kz_k\right)=a_j
$$

are continuous because every linear map on a finite-dimensional normed space is continuous. Hahn--Banach extends each to  
$\ell_j\in Z'$ without increasing its norm, and then

$$
\ell_j(z_k)=\delta_{jk}.
$$

For an arbitrary finite-dimensional subspace $M$, choose a basis $z_1,\ldots,z_n$ and these extended coordinate functionals. Then

$$
N=\bigcap_{j=1}^n\ker\ell_j
$$

is closed. Every $z\in Z$ has the decomposition

$$
z=\sum_j\ell_j(z)z_j+
\left(z-\sum_j\ell_j(z)z_j\right)\in M+N.
$$

Applying every $\ell_j$ shows $M\cap N=\{0\}$, so

$$
\boxed{Z=M\oplus N}.
$$

## ↑ Ancestors (10)

1. [23G](../23g.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
