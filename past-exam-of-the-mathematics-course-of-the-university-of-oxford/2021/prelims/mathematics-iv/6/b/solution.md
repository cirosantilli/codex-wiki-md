<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [b](../b.md)

Continue with $f=p\sin\phi$ and $q=p\cos\phi$. The [tangent vector](../../../../../../tangent-vector-split.md) to the hoop is $\mathbf r_\phi=f'\mathbf e_1-q'\mathbf e_3$. Smooth contact means that the hoop's [normal force](../../../../../../normal-force.md) has zero [dot product](../../../../../../dot-product.md) with this [tangent vector](../../../../../../tangent-vector-split.md). The remaining applied force is $-mg\mathbf e_3$, whose [dot product](../../../../../../dot-product.md) with $\mathbf r_\phi$ is $mgq'$.

Since $\boldsymbol\omega=\omega\mathbf e_3$, the [Coriolis force](../../../../../../coriolis-force.md) is perpendicular to the hoop's [plane](../../../../../../plane.md) and hence to $\mathbf r_\phi$. Also

$$
\boldsymbol\omega\times(\boldsymbol\omega\times\mathbf r)=-\omega^2f\mathbf e_1.
$$

Take the [dot product](../../../../../../dot-product.md) of the rotating-frame [Newton's second law](../../../../../../newton-s-second-law.md) with $\mathbf r_\phi$, substitute [a](../a.md), and divide by $m$:

$$
(f'^2+q'^2)\ddot\phi+(f'f''+q'q'')\dot\phi^2-\omega^2ff'=gq'.
$$

Define

$$
K=f'^2+q'^2,\qquad J=-\frac12\omega^2f^2-gq.
$$

Then $K'/2=f'f''+q'q''$ and $J'=-\omega^2ff'-gq'$, so

$$
\boxed{K(\phi)\ddot\phi+\tfrac12K'(\phi)\dot\phi^2+J'(\phi)=0.}
$$

Expanding the squares makes the cancellation of the mixed terms explicit:

$$
\boxed{K(\phi)=(p'\sin\phi+p\cos\phi)^2+(p'\cos\phi-p\sin\phi)^2=(p')^2+p^2>0.}
$$

The strict [inequality](../../../../../../inequality-mathematics.md) follows from $p>0$. Here $J$ is the [rotating-frame effective potential](../../../../../../rotating-frame-effective-potential.md) per unit [mass](../../../../../../mass.md). Multiplication of the [equation](../../../../../../equation.md) by $\dot\phi$ gives the useful first [integral](../../../../../../integral-split.md) $\tfrac12K(\phi)\dot\phi^2+J(\phi)=\text{constant}$.

## ↑ Ancestors (12)

1. [b](../b.md)
2. [6](../../6.md)
3. [Mathematics IV](../../../mathematics-iv-split.md)
4. [Prelims](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
