<h1 id="6a/solution">Solution</h1>

↑ **Parent:** [6A](../6a.md)

By the [law of mass action](../../../../../law-of-mass-action.md), the net changes in the intermediate concentrations are

$$
\dot X=k_1A-(k_2B+k_4)X+k_3X^2Y,\qquad\dot Y=k_2BX-k_3X^2Y.
$$

The autocatalytic reaction increases $X$ by one and decreases $Y$ by one; its reaction-rate convention is $k_3X^2Y$. With the specified common concentration scale and time scale, choose

$$
\boxed{\alpha=\frac{k_4}{k_1A},\qquad a=\frac{k_3(k_1A)^2}{k_4^3},\qquad b=\frac{k_2B}{k_4}.}
$$

Substitution gives the nondimensional [Brusselator](../../../../../brusselator.md) system. Adding its two steady equations gives $u=1$, and then the second gives $v=b/a$. Its [Jacobian matrix](../../../../../jacobian-matrix.md) there is

$$
J=\begin{pmatrix}b-1&a\\-b&-a\end{pmatrix},\qquad\operatorname{tr}J=b-1-a,\quad\det J=a>0.
$$

The equilibrium is asymptotically stable for $b<1+a$ and unstable for $b>1+a$. At $b_c=1+a$ the [eigenvalues](../../../../../eigenvalue.md) are $\pm i\sqrt a$, crossing the imaginary axis with nonzero speed $\frac d{db}\operatorname{Re}\lambda=1/2$.

The nonlinear [Hopf bifurcation](../../../../../hopf-bifurcation.md) is nondegenerate. At the threshold, put $x=u-1$ and $y=-\sqrt a[(u-1)+(v-b/a)]$. The translated equations are

$$
x'=-\sqrt a\,y+(1-a)x^2-2\sqrt a\,xy-ax^3-\sqrt a\,x^2y,\qquad y'=\sqrt a\,x.
$$

The [Hopf coefficient of the Brusselator](../../../../../hopf-coefficient-of-the-brusselator.md) in the planar radial normalization is $-(a+2)/8<0$: the cubic contribution is $-6a/16$ and the quadratic contribution is $[-2\sqrt a\,2(1-a)]/(16\sqrt a)$. Consequently the bifurcation is supercritical, producing small stable oscillations on the unstable-equilibrium side. Their limiting period is

$$
\boxed{P_\tau\longrightarrow\frac{2\pi}{\sqrt a},\qquad P_t\longrightarrow\frac{2\pi}{k_4\sqrt a}.}
$$

## ↑ Ancestors (10)

1. [6A](../6a.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
