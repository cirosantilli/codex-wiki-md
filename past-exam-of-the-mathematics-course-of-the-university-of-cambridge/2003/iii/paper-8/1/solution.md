<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use the local coordinate $t=1/\lambda$. The differential system becomes

$$
\frac{dy}{dt}=-\left(\frac{A_0}{t^4}+\frac{A_1}{t^3}+\frac{A_2}{t^2}\right)y.
$$

For the nonzero quadratic leading term, the coefficient of the local [linear ordinary differential equation](../../../../../linear-ordinary-differential-equation.md) system has a **[pole](../../../../../pole.md) of order four**, so infinity is an [irregular singular point](../../../../../irregular-singular-point.md) of [Poincaré rank](../../../../../poincare-rank.md) **three** in this gauge. The [matrix](../../../../../matrix.md)-valued function $A(\lambda)$ itself has a [pole](../../../../../pole.md) of order two; the extra factor $d\lambda/dt=-t^{-2}$ is essential when classifying the equation. If $A_0$ vanishes the degree and these orders decrease. The specified distinct [eigenvalues](../../../../../eigenvalue.md) $1,-1$ give the nondegenerate unramified case.

The leading [exponential function](../../../../../exponential-function.md) factors have actions $q_\pm=\pm\lambda^3/3$, so their difference is $2\lambda^3/3$. Equal exponential magnitudes occur on

$$
\boxed{\operatorname{Re}(\lambda^3)=0,\qquad
\arg\lambda=\frac\pi6+\frac{k\pi}3\quad(k=0,\ldots,5).}
$$

These are commonly called Stokes rays in the sectorial ODE convention. With the action-phase convention used by the wiki's [Stokes line](../../../../../stokes-line.md) article they are [anti-Stokes lines](../../../../../anti-stokes-line.md); the same-phase rays instead have

$$
\boxed{\operatorname{Im}(\lambda^3)=0,\qquad\arg\lambda=\frac{k\pi}3.}
$$

Giving both defining equations removes the nomenclature ambiguity; both sets contain six directions.

The standard construction with distinct leading [eigenvalues](../../../../../eigenvalue.md) uses **six [sectorial fundamental solutions](../../../../../sectorial-fundamental-solution.md) per turn**, with basic angular spacing $\pi/3$. They are [fundamental matrices](../../../../../fundamental-matrix-of-a-linear-differential-equation.md), each containing two independent column solutions. On the [logarithm](../../../../../logarithm.md) cover choose six consecutive overlapping sectors of width $\pi/3+2\delta$, with $\delta>\varepsilon/2$ small. Their union has angular opening $2\pi+2\delta$, covering the requested $2\pi+\varepsilon$. One often also writes a seventh index to compare the closing sector with the first after a full turn; that is a closing copy, not a seventh independent sector in the six-sector construction. The number is a generic [sectorial fundamental solution](../../../../../sectorial-fundamental-solution.md) normalization count, not a universal minimum for exceptional systems with vanishing [Stokes matrices](../../../../../stokes-matrix.md): the exactly diagonal system already has one global elementary [fundamental matrix](../../../../../fundamental-matrix-of-a-linear-differential-equation.md).

There is a missing qualification in the requested product identity. [Polynomial](../../../../../polynomial-split.md) coefficients give an entire invertible [fundamental matrix](../../../../../fundamental-matrix-of-a-linear-differential-equation.md), hence trivial actual [monodromy](../../../../../monodromy.md) about a large circle: the circle contracts through [ordinary points](../../../../../ordinary-point-criterion-for-a-second-order-equation.md). But the formal [matrix](../../../../../matrix.md) generally has the form $\widehat G\lambda^\Theta e^Q$, and a positive turn changes its [logarithm](../../../../../logarithm.md) branch by the [formal monodromy](../../../../../formal-monodromy.md) $M_f=e^{2\pi i\Theta}$. This factor cannot be discarded.

To specify the printed product order, let $S_j$ act on column vectors of solution coefficients across the $j$th sector boundary, so adjacent normalized [matrices](../../../../../matrix.md) satisfy $Y_{j+1}=Y_jS_j^{-1}$. Six transitions give $Y_7=Y_1(S_6\cdots S_1)^{-1}$. The normalized formal branch after the turn is $\widehat Y_1M_f$, so sectorial uniqueness gives $Y_7=Y_1M_f$. Consequently

$$
\boxed{S_6S_5S_4S_3S_2S_1=M_f^{-1}=e^{-2\pi i\Theta}.}
$$

Using [Stokes matrices](../../../../../stokes-matrix.md) for right changes of [fundamental matrices](../../../../../fundamental-matrix-of-a-linear-differential-equation.md) instead reverses/inverts the corresponding convention; the [formal monodromy](../../../../../formal-monodromy.md) factor remains necessary. The [formal monodromy correction to an entire-system Stokes product](../../../../../formal-monodromy-correction-to-an-entire-system-stokes-product.md) shows that the printed identity holds when **$M_f=I$**, including the corrected Lax specialization discussed below.

It does not follow from polynomiality alone. For example take

$$
A(\lambda)=\begin{pmatrix}1&0\\0&-1\end{pmatrix}\lambda^2
+\begin{pmatrix}0&1\\-1&0\end{pmatrix}\lambda
+\begin{pmatrix}3/2&1\\2&-3/2\end{pmatrix}.
$$

The coefficient matching in question 2 gives $\Theta=\tfrac12\operatorname{diag}(1,-1)$, hence $M_f=-I$ and the ordered [Stokes matrix](../../../../../stokes-matrix.md) product is $-I$, not $I$, despite having no finite singularity. This is an explicit counterexample to the unqualified final clause.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 8](../../paper-8-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
