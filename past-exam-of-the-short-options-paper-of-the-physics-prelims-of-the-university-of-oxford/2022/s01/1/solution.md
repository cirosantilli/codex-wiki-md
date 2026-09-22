<h1 id="s01/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

**Singularities.** The [complex exponential](../../../../complex-exponential-function.md) factors as $F(z)=e^{z/2}e^{1/(2z)}$. The second factor has an [essential singularity](../../../../essential-singularity.md) at zero, and multiplication by the nonvanishing [holomorphic function](../../../../holomorphic-function-split.md) $e^{z/2}$ does not remove it. There are no other finite [singularities](../../../../complex-singularity.md). On the [Riemann sphere](../../../../riemann-sphere.md), infinity is also an [essential singularity](../../../../essential-singularity.md), since $F(1/\zeta)=F(\zeta)$.

**Symmetry and integral formula.** The identity $F(1/z)=F(z)$ and uniqueness of the [Laurent series](../../../../laurent-series.md) on $0<|z|<\infty$ give $F_{-k}=F_k$ for every integer $k$. The [Laurent coefficient](../../../../laurent-coefficient.md) formula, on the positively oriented [unit circle](../../../../complex-unit-circle.md), gives

$$
F_k=\frac{1}{2\pi i}\oint_{|z|=1}F(z)z^{-k-1}\,dz
=\frac{1}{2\pi}\int_0^{2\pi}e^{\cos\theta}e^{-ik\theta}\,d\theta.
$$

The imaginary part vanishes by the substitution $\theta\mapsto2\pi-\theta$. Hence

$$
\boxed{F_k=F_{-k}=\frac{1}{2\pi}\int_0^{2\pi}e^{\cos\theta}\cos(k\theta)\,d\theta.}
$$

**Polynomial contour integral.** For an integer $n\geq0$ and integer $p$, the [binomial theorem](../../../../binomial-theorem.md) gives $(1+z^2)^n=\sum_{j=0}^n\binom nj z^{2j}$. The [residue theorem](../../../../residue-theorem.md) selects $2j-n-p-1=-1$, that is $j=(n+p)/2$. Therefore the correct complete statement is

$$
\boxed{\frac{1}{2\pi i}\oint_{|z|=1}\frac{(1+z^2)^n}{z^{n+p+1}}\,dz=
\begin{cases}
\displaystyle\frac{n!}{((n-p)/2)!((n+p)/2)!},&n+p\text{ even and }|p|\leq n,\\
0,&\text{otherwise}.
\end{cases}}
$$

The printed nonnegative-integer condition alone misses $j\leq n$. For example $n=0,p=2$ satisfies that condition, but the integral is zero and the displayed factorial $(-1)!$ is undefined.

**Explicit coefficients.** Both [Taylor series](../../../../taylor-series.md) in

$$
e^{z/2}e^{1/(2z)}=\sum_{r,s\geq0}\frac{z^{r-s}}{2^{r+s}r!s!}
$$

converge absolutely and uniformly on every compact annulus away from zero, so their product can be regrouped. For $k\geq0$, put $r=s+k$ and $s=m$. For arbitrary integer $k$, use the already proved symmetry:

$$
\boxed{F_k=\sum_{m=0}^\infty\frac{1}{2^{|k|+2m}m!(|k|+m)!}=I_{|k|}(1).}
$$

Here $I_j$ is a [modified Bessel function](../../../../modified-bessel-function.md). The printed series is directly meaningful for $k\geq0$; for negative $k$ the absolute values, or an appropriately shifted lower summation limit, are essential.

## ↑ Ancestors (12)

1. [1](../1.md)
2. [S01](../../s01.md)
3. [2022](../../../2022-split.md)
4. [Past exam of the short options paper of the physics Prelims of the University of Oxford](../../../split.md)
5. [Short options paper of the physics Prelims of the University of Oxford](../../../../short-options-paper-of-the-physics-prelims-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
