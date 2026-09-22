<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Take the separate oscillator energies

$$
E_i=\frac12(y_i^2+\alpha_i^2x_i^2),\qquad i=1,2.
$$

They depend on disjoint canonical coordinate pairs, so

$$
\{E_1,E_2\}=0,\qquad\{E_i,H\}=0.
$$

Thus they are [first integrals in involution](../../../../../../first-integrals-in-involution.md). Their [differentials](../../../../../../differential-of-a-smooth-map.md)

$$
dE_i=\alpha_i^2x_i\,dx_i+y_i\,dy_i
$$

are nonzero precisely when $(x_i,y_i)\ne(0,0)$ and have disjoint supports. Hence they are [functionally independent](../../../../../../functionally-independent-functions.md) on the specified open set.

To understand all further global [integrals of motion](../../../../../../integral-of-motion.md), use the actions

$$
R_i=E_i/\alpha_i>0,\qquad
x_i=\sqrt{2R_i/\alpha_i}\sin\theta_i,\quad
y_i=\sqrt{2\alpha_iR_i}\cos\theta_i.
$$

Direct differentiation gives $dx_i\wedge dy_i=d\theta_i\wedge dR_i$, so these are [action-angle variables](../../../../../../action-angle-variables.md) with

$$
H=\alpha_1R_1+\alpha_2R_2,\qquad
\dot R_i=0,\quad\dot\theta_i=\alpha_i.
$$

When $\alpha_2/\alpha_1$ is irrational, every orbit is dense in its fixed-action two-dimensional [flat torus](../../../../../../flat-torus.md). One elementary proof samples the orbit at times $2\pi j/\alpha_1$: the first angle returns, and the second undergoes an [irrational rotation](../../../../../../irrational-rotation.md). These samples are dense in the second circle. Allowing a fixed additional time supplies any desired first angle, proving density in the whole [flat torus](../../../../../../flat-torus.md).

A continuous, globally defined [integral of motion](../../../../../../integral-of-motion.md) must have the same value on an orbit and its closure. Therefore it is constant on every fixed-action [flat torus](../../../../../../flat-torus.md). A $C^1$ such integral has the form $F=\phi(R_1,R_2)$, with $\phi$ $C^1$, by evaluating $F$ at a fixed choice of angles. Hence

$$
\boxed{dF=\phi_{R_1}\,dR_1+\phi_{R_2}\,dR_2.}
$$

It cannot be independent of $E_1,E_2$. This proves **there are at most two globally independent differentiable integrals**. If a third global integral were independent at a point on an excluded coordinate plane, independence would persist in a neighbourhood and hence at nearby points of the regular open set, again a contradiction.

The word global matters: on an angular chart, $\alpha_2\theta_1-\alpha_1\theta_2$ is a local [integral of motion](../../../../../../integral-of-motion.md) independent of the actions. It is not single-valued on the [flat torus](../../../../../../flat-torus.md) when the frequency ratio is irrational. Thus the assertion would be false for arbitrary local, rather than global, integrals.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 20](../../../paper-20-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
