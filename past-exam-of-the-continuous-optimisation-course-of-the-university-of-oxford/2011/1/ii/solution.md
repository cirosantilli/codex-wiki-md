<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

All three active constraints force $x_1=2$ and $x_2=4$, which also satisfy $x_1^2+x_2^2=20$. For maximization use $\mathcal L=F+\lambda^Tg$, $\lambda\geq0$. At $x^*=(2,4)$,

$$
\nabla F=(16,10),\quad \nabla g_1=(-1,0),\quad
\nabla g_2=(-4,-8),\quad\nabla g_3=(-4,1).
$$

Stationarity gives the complete family

$$
\boxed{\lambda_2=t,\quad\lambda_3=8t-10,\quad\lambda_1=56-36t,
\qquad\frac54\leq t\leq\frac{14}{9}.}
$$

In particular $(\lambda_1,\lambda_2,\lambda_3)=(2,3/2,2)$ is strictly positive. Three [gradients](../../../../gradient.md) in two [dimensions](../../../../dimension-vector-space.md) cannot be linearly independent, so the [linear independence constraint qualification](../../../../linear-independence-constraint-qualification.md) fails. But $d=(-1,-1)$ gives $\nabla g_i\cdot d=(1,12,3)>0$, so the [Mangasarian–Fromovitz constraint qualification](../../../../mangasarian-fromovitz-constraint-qualification.md) holds.

For a nonzero linearized feasible direction $d$, each $\nabla g_i\cdot d\geq0$, and

$$
\nabla F\cdot d=-2\nabla g_1\cdot d-\tfrac32\nabla g_2\cdot d-2\nabla g_3\cdot d<0.
$$

The inequality is strict because equality would require all three inner products to vanish, and the first and third [gradients](../../../../gradient.md) already span $\mathbb R^2$. This proves a strict [local maximum](../../../../local-maximum.md): otherwise a sequence of nearby feasible points with no smaller objective would, after normalizing their differences from $x^*$ and taking a convergent subsequence, give a unit linearized feasible direction with nonnegative objective derivative, contradicting the displayed inequality. Thus

$$
\boxed{x^*=(2,4)\text{ is a strict local maximizer},\quad F(x^*)=32.}
$$

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the continuous optimisation course of the University of Oxford](../../../split.md)
5. [Continuous optimisation course of the University of Oxford](../../../../continuous-optimisation-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
