<h1 id="1/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The two wall [boundary conditions](../../../../../boundary-condition.md) are

$$
\boxed{\hat u=0,\qquad \hat w=0\quad(z=0).}
$$

Define the [capillary parameter for a falling film](../../../../../capillary-parameter-for-a-falling-film.md)

$$
\boxed{S=\frac{2\gamma}{3\rho gL^2\sin\alpha}.}
$$

Retain $S=O(1)$ in the [long-wave approximation](../../../../../long-wave-approximation.md). Thus [surface tension](../../../../../surface-tension-split.md) is retained in the leading [normal stress](../../../../../normal-stress.md) balance even though geometric slope corrections are small. For $h_x=O(1)$ in the rescaled coordinates, the dimensional surface slope is $\varepsilon h_x$.

The three [free surface](../../../../../free-surface.md) [boundary conditions](../../../../../boundary-condition.md), accurate through $O(\varepsilon)$, are

$$
\boxed{\begin{aligned}
h_t+(\bar u+\hat u)h_x&=\hat w,\\
\bar u_z+\hat u_z&=0,\\
\hat p&=(h-1)\cot\alpha-\frac32S h_{xx}+\varepsilon\hat w_z,
\end{aligned}\qquad z=h(x,t).}
$$

The first is the [kinematic boundary condition](../../../../../kinematic-boundary-condition.md); the second is the zero tangential [traction](../../../../../traction.md) condition. For the third, the dimensional liquid-side [pressure](../../../../../pressure-split.md) is, to the required order,

$$
p-p_a=-\gamma\frac{h_0}{L^2}h_{xx}
+\frac{2\mu\varepsilon U_0}{h_0}w_z.
$$

Division by $\rho gh_0\sin\alpha$ gives $p=-3S h_{xx}/2+\varepsilon w_z$ in dimensionless variables. Subtracting $\bar p(h)=(1-h)\cot\alpha$ gives the stated perturbation condition. The additional slope-times-shear contribution to [normal stress](../../../../../normal-stress.md) vanishes at this order because the tangential [traction](../../../../../traction.md) is zero. The omitted geometric and tangential-stress corrections are $O(\varepsilon^2)$ under this ordering.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the topics in fluid mechanics course of the University of Oxford](../../../../split.md)
6. [Topics in fluid mechanics course of the University of Oxford](../../../../../topics-in-fluid-mechanics-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
