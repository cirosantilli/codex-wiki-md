<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Put $\nu=k/\delta$ and use the [discrete Fourier transform](../../../../../../discrete-fourier-transform.md) on the infinite grid. A spatial [Fourier mode](../../../../../../fourier-mode.md) $e^{i(j\theta+\ell\phi)}$ has time coefficient satisfying

$$
v_{n+1}=2is\,v_n+v_{n-1},\qquad s=\nu(\sin\theta+\sin\phi).
$$

Its [amplification polynomial of a multilevel finite difference scheme](../../../../../../amplification-polynomial-of-a-multilevel-finite-difference-scheme.md) is $\zeta^2-2is\zeta-1$, with roots

$$
\zeta_\pm=is\pm\sqrt{1-s^2}.
$$

For $|s|<1$ they are distinct and have modulus one. Since $|s|\leq2\nu$, a fixed $0<\nu<1/2$ bounds their separation below by $2\sqrt{1-4\nu^2}$. Solving for the two mode amplitudes therefore bounds every power of the two-level [companion matrix](../../../../../../companion-matrix.md) uniformly in frequency and step number. [Parseval identity](../../../../../../parseval-identity.md) transfers this bound to the [discrete L2 norm](../../../../../../discrete-l2-norm.md).

If $\nu>1/2$, an open set of frequencies around $(\pi/2,\pi/2)$ has $|s|>1$ and a root of modulus greater than one. Fourier data supported there grow exponentially. At $\nu=1/2$, the central frequency has the double root $i$, and the recurrence admits $v_n=(A+Bn)i^n$. Thus the root moduli being one do not suffice: a nontrivial [Jordan block](../../../../../../jordan-block.md) makes the two-level powers grow linearly. Although this exact frequency has measure zero on the infinite grid, the [matrices](../../../../../../matrix.md) depend continuously on frequency. For every step count, a neighborhood has powers nearly as large, so their essential supremum is still unbounded. Wave packets in those neighborhoods rule out a uniform [stability of a numerical method](../../../../../../stability-of-a-numerical-method.md) estimate in the [discrete L2 norm](../../../../../../discrete-l2-norm.md).

For arbitrary perturbations in both starting levels the sharp positive range is therefore

$$
\boxed{0<\Delta t/\Delta x<1/2.}
$$

The zero-step limiting recurrence is bounded but does not advance time. A specially filtered startup can suppress a repeated-root mode; that restriction does not establish stability of the full two-level scheme. This is the [two-dimensional leapfrog stability threshold](../../../../../../two-dimensional-leapfrog-stability-threshold.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 67](../../../paper-67-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
