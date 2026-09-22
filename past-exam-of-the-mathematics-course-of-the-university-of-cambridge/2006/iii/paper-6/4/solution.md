<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Set $a_n=\|x^n\|$ and $D=\inf_{n\ge1}a_n^{1/n}$. If some $x^m=0$, all later powers vanish, their root [norms](../../../../../norm.md) tend to zero, and $D=0$. Otherwise fix $m\ge1$ and write $n=qm+s$, $0\le s<m$. [Submultiplicativity](../../../../../submultiplicativity.md) gives

$$
a_n\le a_m^q C_m,\qquad C_m=\max_{0\le s<m}\|x^s\|.
$$

Since $q/n\to1/m$, it follows that $\limsup_na_n^{1/n}\le a_m^{1/m}$. Taking the infimum over $m$ and using $a_n^{1/n}\ge D$ proves

$$
\lim_{n\to\infty}\|x^n\|^{1/n}=D.
$$

This establishes existence of the limit and its infimum characterization before identifying it with the [spectral radius](../../../../../spectral-radius.md) $r(x)=\max_{\lambda\in\sigma(x)}|\lambda|$.

For $|\lambda|>D$, the [root test](../../../../../root-test.md) makes $\sum_{n\ge0}x^n/\lambda^{n+1}$ converge absolutely. Multiplication of partial sums shows that its limit is $(\lambda1-x)^{-1}$. Thus $r(x)\le D$. For the reverse inequality, take any $\rho>r(x)$ and the circle $|\lambda|=\rho$. The [resolvent of an element](../../../../../resolvent-of-an-element.md) is holomorphic off the [spectrum](../../../../../spectrum-functional-analysis.md), and

$$
x^n=\frac1{2\pi i}\int_{|\lambda|=\rho}\lambda^n(\lambda1-x)^{-1}\,d\lambda.
$$

To justify this identity, first use a radius larger than $\|x\|$ and integrate the uniformly convergent [Neumann series](../../../../../neumann-series.md) term by term. Then deform to radius $\rho$: the intervening annulus has no spectral points. The [Cauchy theorem](../../../../../cauchy-s-integral-theorem.md) for these Banach-valued integrals follows by applying [bounded linear functionals](../../../../../continuous-linear-functional.md) and using their point separation. Consequently, with $M_\rho=\max_{|\lambda|=\rho}\|(\lambda1-x)^{-1}\|$,

$$
\|x^n\|\le\rho^{n+1}M_\rho.
$$

Taking root limits gives $D\le\rho$; let $\rho\downarrow r(x)$. Hence the full [spectral radius formula](../../../../../spectral-radius-formula.md) is

$$
\boxed{r(x)=\lim_{n\to\infty}\|x^n\|^{1/n}
=\inf_{n\ge1}\|x^n\|^{1/n}.}
$$

For the product comparison, if $\lambda\ne0$ and $R=(\lambda1-xy)^{-1}$, direct multiplication on both sides verifies

$$
(\lambda1-yx)^{-1}=\lambda^{-1}(1+yRx).
$$

Indeed $(\lambda1-yx)y=y(\lambda1-xy)$, and the remaining terms cancel against the inverse equation. Interchanging $x,y$ proves the converse. Thus the [nonzero spectra of products in opposite orders](../../../../../nonzero-spectra-of-products-in-opposite-orders.md) agree, so

$$
\boxed{r(xy)=r(yx).}
$$

The possible difference at zero has no effect on the maximum modulus, including when that maximum is zero.

Zero really can differ. In $A=\mathcal B(\ell^2(\mathbb N_0))$, let $S$ be the [unilateral shift operator](../../../../../unilateral-shift-operator.md), $Se_n=e_{n+1}$, and take $x=S^*$, $y=S$. Then $xy=1$, whereas $yx=1-P_0$, with $P_0$ the projection onto $e_0$. The latter is zero on $e_0$ and identity on its orthogonal complement, and these blocks also explicitly invert it away from zero and one. Hence

$$
\boxed{\sigma(xy)=\{1\},\qquad\sigma(yx)=\{0,1\}.}
$$

Finally, for $t>r(x)$ the root [norms](../../../../../norm.md) of $(x/t)^n$ tend to $r(x)/t<1$, so their [norms](../../../../../norm.md) eventually decay geometrically and the powers converge to zero. Conversely, if the powers converge to zero, choose $N$ with $\|(x/t)^N\|<1$. Homogeneity and the infimum formula imply

$$
\frac{r(x)}t\le\|(x/t)^N\|^{1/N}<1,
$$

so $t>r(x)$. The admissible positive $t$ are exactly $(r(x),\infty)$, proving the [power-decay characterization of the spectral radius](../../../../../power-decay-characterization-of-the-spectral-radius.md)

$$
\boxed{r(x)=\inf\{t>0:(t^{-1}x)^n\to0\}.}
$$

This includes quasinilpotent elements with radius zero; no positive endpoint must be attained.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 6](../../paper-6-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
