<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

At large $|\zeta|$, $z=\zeta+O(\zeta^{-1})$, so the map tends to the identity. Its exterior inverse has the expansion $\zeta=z-a^2/z+O(z^{-3})$. Therefore the physical [complex potential of a two-dimensional potential flow](../../../../complex-potential-of-a-two-dimensional-potential-flow.md) is $w(z)=W(\zeta(z))$, with

$$
w(z)=Ue^{-i\alpha}z+\frac{U(e^{i\alpha}-a^2e^{-i\alpha})}{z}+O(z^{-3}).
$$

Its leading term is unchanged, so the far-field [velocity](../../../../velocity.md) still has magnitude $U$ and inclination $\alpha$.

The [chain rule](../../../../chain-rule.md) gives the [complex velocity](../../../../complex-velocity.md):

$$
\boxed{u-iv=\frac{dW/d\zeta}{dz/d\zeta}
=U\frac{e^{-i\alpha}-e^{i\alpha}/\zeta^2}{1-a^2/\zeta^2}
=U\frac{e^{-i\alpha}\zeta^2-e^{i\alpha}}{\zeta^2-a^2}.}
$$

The parameter $\zeta$ denotes the unique exterior preimage of $z$. If an expression solely in $z$ is desired, take

$$
\zeta(z)=\frac{z+\sqrt{z^2-4a^2}}2,
$$

where the exterior [holomorphic square root](../../../../holomorphic-square-root.md) is chosen so that $\sqrt{z^2-4a^2}\sim z$ at infinity. Its branch points lie inside the [ellipse](../../../../ellipse.md). This is [uniform potential flow around an ellipse](../../../../uniform-potential-flow-around-an-ellipse.md).

## ↑ Ancestors (12)

1. [D](../d.md)
2. [2](../../2.md)
3. [2014](../../../2014-split.md)
4. [Past exam of the fluids and waves course of the University of Oxford](../../../split.md)
5. [Fluids and waves course of the University of Oxford](../../../../fluids-and-waves-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
