<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [first Jackson theorem for periodic approximation](../../../../../../first-jackson-theorem-for-periodic-approximation.md) states that an absolute constant $C_J$ exists such that, for every continuous $2\pi$-periodic [function](../../../../../../function-split.md) $g$ and integer $n\ge1$, there is a [trigonometric polynomial](../../../../../../trigonometric-polynomial.md) $q_n$ of degree at most $n$ satisfying

$$
\|g-q_n\|_\infty\le C_J\omega(g,1/n).
$$

Apply it to the continuous periodic [function](../../../../../../function-split.md) $g(\theta)=f(\cos\theta)$, which is even. Replace the approximant by its even part

$$
q_n^{\rm ev}(\theta)=\frac12\bigl(q_n(\theta)+q_n(-\theta)\bigr).
$$

Since $g(-\theta)=g(\theta)$, the [triangle inequality](../../../../../../triangle-inequality.md) gives $\|g-q_n^{\rm ev}\|_\infty\le\|g-q_n\|_\infty$. This symmetrization cancels all sine terms, so $q_n^{\rm ev}=\sum_{j=0}^n\alpha_j\cos(j\theta)$. The [Chebyshev polynomials](../../../../../../chebyshev-polynomial.md) satisfy $T_j(\cos\theta)=\cos(j\theta)$ and have degree $j$; the latter follows inductively from $T_0=1$, $T_1=x$ and $T_{j+1}=2xT_j-T_{j-1}$. Therefore

$$
p_n(x)=\sum_{j=0}^n\alpha_jT_j(x)
$$

is an algebraic [polynomial](../../../../../../polynomial-split.md) of degree at most $n$, and $p_n(\cos\theta)=q_n^{\rm ev}(\theta)$. Because cosine maps onto $[-1,1]$, the [supremum norms](../../../../../../supremum-norm.md) agree exactly:

$$
\|f-p_n\|_{[-1,1]}=\|g-q_n^{\rm ev}\|_{\mathbb T}.
$$

Finally, the definition of the best error, periodic Jackson approximation, and part (a) give the successive bounds

$$
E_n(f)\le\|f-p_n\|_\infty
\le C_J\omega(g,1/n)
\le C_J\omega(f,1/n).
$$

Thus

$$
\boxed{E_n(f)\le C_J\omega(f,1/n),\qquad n\ge1.}
$$

Neither the constant nor the choice of approximation space depends on $f$. The [cosine substitution for polynomial approximation](../../../../../../cosine-substitution-for-polynomial-approximation.md) and even symmetrization are what preserve the required degree bound.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 75](../../../paper-75-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
