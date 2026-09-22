<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

To illustrate [Tikhonov regularization](../../../../../../tikhonov-regularization.md) precisely, take the unknown to be the trace $g$ on a chosen enclosing sphere of radius $R$. Use [Hilbert spaces](../../../../../../hilbert-space-split.md) $X=Y=L^2(S^2)$ and the forward [linear operator](../../../../../../linear-operator.md)

$$
(Ag)_n^m=\frac{g_n^m}{d_n},\qquad d_n=ki^{n+1}h_n^{(1)}(kR).
$$

At real positive $kR$, $d_n\ne0$, because the real [Spherical Bessel functions](../../../../../../spherical-bessel-function.md) $j_n,y_n$ have a nonzero [Wronskian](../../../../../../wronskian.md) and cannot vanish simultaneously. Moreover $|d_n|\to\infty$. Thus $A$ is an injective [compact operator](../../../../../../compact-operator-split.md): truncating to finitely many harmonic orders approximates it in [operator norm](../../../../../../operator-norm.md), since the remaining diagonal entries tend uniformly to zero. Its inverse is unbounded. This is a linear field reconstruction; estimating the obstacle from the reconstructed field remains a further nonlinear step.

Given coefficients $b_n^m$ of measured data $y^\delta$, minimize the quadratic functional

$$
\|Ag-y^\delta\|^2+\alpha\|g\|^2,\qquad\alpha>0.
$$

Varying $g$ in every direction gives $(A^*A+\alpha I)g_\alpha^\delta=A^*y^\delta$. The operator $A^*A+\alpha I$ is bounded below by $\alpha I$, so it is invertible and the minimizer is unique. In coefficients the minimization is separable: $A^*y$ has coefficient $b_n^m/\overline{d_n}$ and $A^*A$ has multiplier $|d_n|^{-2}$. Hence the [Tikhonov regularization of spherical far-field continuation](../../../../../../tikhonov-regularization-of-spherical-far-field-continuation.md) is

$$
\boxed{(g_\alpha^\delta)_n^m=\frac{d_n b_n^m}{1+\alpha|d_n|^2}.}
$$

The implied regularized far-field coefficients are $b_n^m/(1+\alpha|d_n|^2)$. This suppresses precisely the high-order coefficients that make backward continuation unstable.

Let $g^\dagger$ be the exact trace and $y=Ag^\dagger$, with $\|y^\delta-y\|\le\delta$. The [noise-bias decomposition for linear regularization](../../../../../../noise-bias-decomposition-for-linear-regularization.md) is

$$
g_\alpha^\delta-g^\dagger=(A^*A+\alpha I)^{-1}A^*(y^\delta-y)-\alpha(A^*A+\alpha I)^{-1}g^\dagger.
$$

For a [singular value](../../../../../../singular-value.md) $s=|d_n|^{-1}$, the noise multiplier is $s/(s^2+\alpha)$. Since $s^2+\alpha\ge2s\sqrt\alpha$, its supremum is at most $1/(2\sqrt\alpha)$. Consequently

$$
\boxed{\|g_\alpha^\delta-g^\dagger\|\le\frac{\delta}{2\sqrt\alpha}+B(\alpha),\qquad
B(\alpha)=\left\|\alpha(A^*A+\alpha I)^{-1}g^\dagger\right\|.}
$$

This [Tikhonov stability bound](../../../../../../tikhonov-stability-bound.md) measures the trace [norm](../../../../../../norm.md), not a distance between obstacle boundaries. The bias coefficient is $\alpha/(|d_n|^{-2}+\alpha)$ times the exact coefficient. It tends to zero for each fixed $n,m$, is bounded by one, and $\sum|g_n^{\dagger,m}|^2<\infty$. Splitting off a finite sum and bounding its tail therefore proves $B(\alpha)\to0$ as $\alpha\to0$.

A convergent [regularization parameter choice](../../../../../../regularization-parameter-choice.md) thus satisfies

$$
\boxed{\alpha(\delta)\to0,\qquad\frac{\delta}{\sqrt{\alpha(\delta)}}\to0.}
$$

In nondimensionalized variables, $\alpha=\delta^p$ with $0<p<2$ is one such rule. Without a smoothness assumption on the exact trace there is no universal bias rate and no universal optimal value of $\alpha$. For a concrete [normal-operator source condition](../../../../../../normal-operator-source-condition.md), suppose $g^\dagger=A^*Aw$ and $\|w\|\le C$. Each bias multiplier on $w$ is $\alpha s^2/(s^2+\alpha)\le\alpha$, so $B(\alpha)\le C\alpha$. Minimizing the resulting bound gives, for $C>0$,

$$
\frac{d}{d\alpha}\left(C\alpha+\frac{\delta}{2\sqrt\alpha}\right)=C-\frac{\delta}{4\alpha^{3/2}},\qquad
\boxed{\alpha=\left(\frac{\delta}{4C}\right)^{2/3},\quad\|g_\alpha^\delta-g^\dagger\|=O(C^{1/3}\delta^{2/3}).}
$$

This optimizes the displayed worst-case bound under that additional source condition, rather than guaranteeing an exact optimum for every datum.

If only the effect of measurement error is minimized, the multiplier bound decreases when $\alpha$ increases. Indeed $\|(A^*A+\alpha I)^{-1}A^*\|\le\|A\|/\alpha\to0$ as $\alpha\to\infty$. But the reconstruction then approaches zero and its bias approaches $\|g^\dagger\|$. **Suppressing noise alone does not optimize reconstruction: $\alpha$ must balance noise amplification against regularization bias.** A geometrically accurate obstacle estimate additionally needs justified shape constraints and a stable procedure for extracting a boundary from the regularized field.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 80](../../../paper-80-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
