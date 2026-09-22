<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

In first Born order the unknown potential enters linearly. Let $M_i$ multiply by the known incident field, $\mathcal G$ be the outgoing Green [integral](../../../../../../integral.md) over the known support $D$, and $\mathcal R$ restrict the resulting field to the measurement set. With $y$ the measured scattered data,

$$
\boxed{y=AV,\qquad A=\mathcal R\mathcal G M_i.}
$$

The formal least-squares, [minimum-norm least-squares solution](../../../../../../minimum-norm-least-squares-solution.md) is $V=A^\dagger y$, or $V=(A^*A)^{-1}A^*y$ on a domain where that inverse is meaningful. The [refractive index](../../../../../../refractive-index.md) is then

$$
\boxed{n(\mathbf r)=\sqrt{1+V(\mathbf r)/k^2},}
$$

choosing the physical branch approaching one outside the scatterer. At weak contrast $n-1\simeq V/(2k^2)$.

A noisy stable reconstruction uses [Tikhonov regularization](../../../../../../tikhonov-regularization.md):

$$
V_\alpha^\delta=\operatorname*{arg\,min}_V\left\{\|AV-y^\delta\|_Y^2+\alpha\|V\|_X^2\right\},\qquad
\boxed{V_\alpha^\delta=(A^*A+\alpha I)^{-1}A^*y^\delta,\quad\alpha>0.}
$$

A smoothness penalty $\alpha\|LV\|^2$ may be substituted when appropriate, giving $A^*A+\alpha L^*L$ in the [normal equation for a linear inverse problem](../../../../../../normal-equation-for-a-linear-inverse-problem.md), under the corresponding [coercivity](../../../../../../coercive-function.md) assumptions. The parameter balances noise amplification and smoothing bias.

The data geometry matters: knowing a [scattered field](../../../../../../scattered-wave.md) on a measurement surface does not automatically mean knowing it throughout the support. A single incident wave and fixed-frequency far field sample only a shifted sphere of the potential's [Fourier transform](../../../../../../fourier-transform.md), and in general do not determine an arbitrary three-dimensional potential uniquely. [Tikhonov regularization](../../../../../../tikhonov-regularization.md) stabilizes a selected [minimum-norm least-squares solution](../../../../../../minimum-norm-least-squares-solution.md); it cannot create missing information or guarantee uniqueness from inadequate data. If the total field and its [derivatives](../../../../../../derivative.md) were known throughout $D$, the first-Born equation could instead be inverted formally as $V\simeq-(\Delta+k^2)\psi_s/\psi_i$ where $\psi_i\ne0$, but differentiation still amplifies measurement noise.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 70](../../../paper-70-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
