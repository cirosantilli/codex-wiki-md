<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

For a positively oriented simple closed [contour](../../../../complex-integration-contour.md) $C$, with no [pole](../../../../pole.md) on $C$ and with $f$ [holomorphic](../../../../holomorphic-function-split.md) inside except at finitely many poles, the [residue theorem](../../../../residue-theorem.md) states

$$
\oint_Cf(z)\,dz=2\pi i\sum_{z_j\text{ inside }C}\operatorname{Res}(f,z_j).
$$

For a more general closed contour, each [residue](../../../../residue.md) is multiplied by its [winding number](../../../../winding-number.md) about the pole.

The powers must be defined using the same [branch of the complex logarithm](../../../../branch-of-the-complex-logarithm.md) as the numerator. A branch suitable for both requested calculations is

$$
\operatorname{Log}z=\log|z|+i\arg z,\qquad -\delta<\arg z<2\pi-\delta,
\quad 0<\delta<2\pi-\max\left(\pi,\frac{2\pi}{\beta}\right).
$$

The [branch cut](../../../../branch-cut.md) is a ray just below the positive real axis, and $z^\beta:=e^{\beta\operatorname{Log}z}$. Since $\beta>1$, the displayed choice of $\delta$ is possible. It includes the required upper half-plane and the sector used below. The origin remains an excluded [branch point](../../../../branch-point.md).

In $0\leq\arg z<\pi$, all zeros of $1+z^\beta$ are

$$
\zeta_j=\exp\frac{(2j+1)\pi i}{\beta},\qquad j=0,1,\ldots,\quad 2j+1<\beta.
$$

Each is a [simple pole](../../../../simple-pole.md), since $\beta\zeta_j^{\beta-1}=-\beta/\zeta_j\ne0$. Its [residue](../../../../residue.md) is

$$
\boxed{\operatorname{Res}(f,\zeta_j)=-\frac{\zeta_j\operatorname{Log}\zeta_j}{\beta}=-\frac{i(2j+1)\pi}{\beta^2}\exp\frac{(2j+1)\pi i}{\beta}.}
$$

The strict inequality matters if a root lies on the negative real axis, which is outside the specified region.

To evaluate the two [improper integrals](../../../../improper-integral.md), write them as $I$ for the logarithmic numerator and $J$ for numerator one, and set $\theta=\pi/\beta$, $\alpha=2\theta$. Use a counterclockwise annular sector with $\epsilon<|z|<R$ and $0<\arg z<\alpha$. It encloses precisely $\zeta_0=e^{i\theta}$. The outward positive-axis segment contributes $I$ in the limit. On the inward segment $z=re^{i\alpha}$, the logarithm is $\log r+i\alpha$ and $z^\beta=r^\beta$, so that segment contributes $-e^{i\alpha}(I+i\alpha J)$.

The small arc is $O(\epsilon|\log\epsilon|)$, and the large arc is $O(R^{1-\beta}\log R)$; both vanish. These estimates follow from the arc lengths and $|1+z^\beta|\geq\big||z|^\beta-1\big|$. The real integrals also converge absolutely at both endpoints for $\beta>1$. The [residue theorem](../../../../residue-theorem.md) now gives

$$
(1-e^{2i\theta})I-2i\theta e^{2i\theta}J=2\theta^2e^{i\theta}.
$$

After division by $e^{i\theta}$, the real and imaginary parts are

$$
2\theta\sin\theta\,J=2\theta^2,\qquad -2\sin\theta\,I-2\theta\cos\theta\,J=0.
$$

Since $0<\theta<\pi$, $\sin\theta>0$. Hence the [logarithmic beta integral from a sector contour](../../../../logarithmic-beta-integral-from-a-sector-contour.md) yields

$$
\boxed{J=\frac{\pi}{\beta\sin(\pi/\beta)},\qquad I=-\frac{\pi^2\cos(\pi/\beta)}{\beta^2\sin^2(\pi/\beta)}.}
$$

For $1<\beta<2$ the sector angle exceeds $\pi$. This is why choosing the [principal complex logarithm](../../../../principal-complex-logarithm.md) on the whole sector would be invalid; the displaced cut above handles that range as well as $\beta\geq2$.

## ↑ Ancestors (12)

1. [4](../4.md)
2. [Paper 2](../../paper-2-split.md)
3. [2011](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
