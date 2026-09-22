<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The dot product of the two [magnetizations](../../../../../../magnetization.md) is $\bar m^2\cos[\theta(x)-\theta(0)]$. For the Gaussian [spin wave](../../../../../../spin-wave.md) field, the [Gaussian phase averaging](../../../../../../gaussian-phase-averaging.md) identity $\langle e^{iX}\rangle=e^{-\langle X^2\rangle/2}$ for a centered Gaussian variable gives

$$
\langle\mathbf m(x)\cdot\mathbf m(0)\rangle
=\bar m^2\exp[-D(r)/2],\qquad
D(r)=\langle[\theta(x)-\theta(0)]^2\rangle=2[G(0)-G(r)].
$$

Keeping this exponential is essential: expanding the cosine to quadratic order would fail when phase differences grow with separation. Equivalently, the [phase-difference variance](../../../../../../phase-difference-variance.md) is

$$
D(r)=\frac2{\bar K}\int\frac{d^dq}{(2\pi)^d}\frac{1-\cos(q\cdot x)}{q^2}.
$$

For $d>2$, the integral defining the absolute phase variance is finite at small momentum after fixing the uniform mode; its microscopic [ultraviolet cutoff](../../../../../../ultraviolet-cutoff.md) still matters. Its nonconstant [Green function](../../../../../../green-s-function.md) decays as $r^{2-d}$, so $D(r)$ tends to a finite constant $D_\infty$ and

$$
\boxed{\lim_{r\to\infty}\langle\mathbf m(x)\cdot\mathbf m(0)\rangle
=m_0^2=\bar m^2e^{-D_\infty/2}>0\quad(d>2).}
$$

In two dimensions, the logarithmic [Green function](../../../../../../green-s-function.md) gives $D(r)=(\pi\bar K)^{-1}\log(r/a)+O(1)$. Consequently

$$
\langle\mathbf m(x)\cdot\mathbf m(0)\rangle\asymp\bar m^2(r/a)^{-1/(2\pi\bar K)}\longrightarrow0.
$$

For $1\le d<2$, $D(r)$ grows as $2r^{2-d}/[(2-d)S_d\bar K]$, up to bounded microscopic terms, and the [correlation function](../../../../../../correlation-function.md) again vanishes. In particular, in one dimension $S_1=2$ gives $D(r)=r/\bar K$ and exponential decay $\bar m^2e^{-r/(2\bar K)}$. Therefore **there is no conventional long-range order for $d\le2$ at positive temperature in this short-range continuous-symmetry model**. In two dimensions, algebraic decay can still support [quasi-long-range order](../../../../../../quasi-long-range-order.md).

These [infrared spin-wave correlations of the XY model](../../../../../../infrared-spin-wave-correlations-of-the-xy-model.md) explain the mechanism behind the [Mermin-Wagner theorem](../../../../../../mermin-wagner-theorem.md). They are a test of the low-temperature [spin wave](../../../../../../spin-wave.md) approximation, not a claim that every $d>2$ [XY model](../../../../../../xy-model.md) is ordered at every temperature. Large local fluctuations and defects destroy the ordered phase at sufficiently high temperature. Also, the assumed small angle is a local smooth-field approximation; phase differences at arbitrarily large separation need not remain small.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 72](../../../paper-72-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
