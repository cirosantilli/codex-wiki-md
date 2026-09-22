<h1 id="9/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Take $s$ positive uphill, $X$ positive to the right, and the cylinder's rotation positive anticlockwise. Contact with the fixed-angle surface determines its normal position; no slipping gives $\dot\theta=-\dot s/R$. These two constraints leave $X,s$ as the two independent coordinates of the [cylinder rolling on a freely translating wedge](../../../../cylinder-rolling-on-a-freely-translating-wedge.md).

The cylinder centre is at $(X+s\cos\alpha-R\sin\alpha,\ s\sin\alpha+R\cos\alpha)$. Since the angle is constant, its squared [speed](../../../../speed.md) is $\dot X^2+2\dot X\dot s\cos\alpha+\dot s^2$. Including the block's [kinetic energy](../../../../kinetic-energy.md) and $I_c=M_cR^2/2$, and dropping a constant from the potential, gives

$$
\boxed{L=\frac12(M_b+M_c)\dot X^2+M_c\cos\alpha\,\dot X\dot s+\frac34M_c\dot s^2-M_cgs\sin\alpha.}
$$

The [cyclic coordinate](../../../../cyclic-coordinate.md) is $X$. Its conserved [conjugate momentum](../../../../canonical-momentum.md) is $p_X=(M_b+M_c)\dot X+M_c\cos\alpha\dot s$, the total horizontal [momentum](../../../../momentum-split.md). The two [Euler-Lagrange equations](../../../../euler-lagrange-equation.md) are

$$
(M_b+M_c)\ddot X+M_c\cos\alpha\ddot s=0,\qquad
\cos\alpha\ddot X+\frac32\ddot s=-g\sin\alpha.
$$

Eliminating the accelerations, with $D=3(M_b+M_c)-2M_c\cos^2\alpha>0$, gives

$$
\boxed{\ddot s=-\frac{2(M_b+M_c)g\sin\alpha}{D},\qquad
\ddot X=\frac{2M_cg\sin\alpha\cos\alpha}{D}.}
$$

Thus the cylinder rolls downhill and the wedge accelerates rightward. For $M_b\gg M_c$, $\ddot X\to0$ and $\ddot s\to-(2/3)g\sin\alpha$, the ordinary fixed-incline result.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [9](../../9.md)
3. [2019](../../../2019-split.md)
4. [Past exam of the physics 1 paper of the University of Oxford](../../../split.md)
5. [Physics 1 paper of the University of Oxford](../../../../physics-1-paper-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
