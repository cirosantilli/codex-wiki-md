<h1 id="3/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Use the scaled [proximal operator](../../../../../../proximal-operator.md) $\operatorname{prox}_{\gamma E}$; take $\gamma=1$ for each unscaled resolvent.

For the quadratic case, write $D^TD=\operatorname{diag}(d_1,\ldots,d_n)$ and $\xi=Qx$. Since $Q$ is an [orthogonal matrix](../../../../../../orthogonal-matrix.md), the quadratic proximal term becomes $\|\xi-Qz\|^2/2$. The [subgradient optimality condition](../../../../../../subgradient-optimality-condition.md) gives

$$
(I+\gamma D^TD)\xi=Qz+\gamma D^Ty.
$$

All $d_j\geq0$, so each diagonal entry is positive, including when $d_j=0$. Multiplying by the inverse [diagonal matrix](../../../../../../diagonal-matrix.md) gives

$$
\boxed{\operatorname{prox}_{\gamma E}(z)=Q^T\operatorname{diag}\left(\frac1{1+\gamma d_j}\right)(Qz+\gamma D^Ty).}
$$

The [proximal operator of Poisson data fidelity](../../../../../../proximal-operator-of-poisson-data-fidelity.md) separates pointwise. At each $t$, the scalar optimality equation on $x>0$ is

$$
x-z+\gamma\left(1-\frac yx\right)=0,\qquad x^2+(\gamma-z)x-\gamma y=0.
$$

Since $y>0$, the two roots have opposite signs. **Only the positive root is admissible** in the logarithm:

$$
\boxed{\operatorname{prox}_{\gamma E}(z)(t)=\frac{z(t)-\gamma+\sqrt{(z(t)-\gamma)^2+4\gamma y(t)}}2.}
$$

The negative root is outside the effective domain. The second derivative $1+\gamma y/x^2$ of the proximal objective is positive, establishing the unique pointwise minimizer. The integral formula is understood on the function spaces where these quantities are admissible.

Finally, for $E(x)=|x|$, positive and negative minimizers obey $x-z+\gamma=0$ and $x-z-\gamma=0$, respectively. At zero the [subdifferential](../../../../../../subdifferential.md) condition is $z\in[-\gamma,\gamma]$. Combining these cases yields [soft thresholding](../../../../../../soft-thresholding.md):

$$
\boxed{\operatorname{prox}_{\gamma|\cdot|}(z)=\operatorname{sgn}(z)\max\{|z|-\gamma,0\}.}
$$

Thus $\gamma=1$ supplies all three requested closed forms.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [3](../../3.md)
3. [Paper 326](../../../paper-326-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
