<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For uniqueness, subtract two solutions and call their difference $w$. It has zero boundary and initial data, with $w_t=w_{xx}+aw_x+bw$. Its squared [L2 norm](../../../../../../l2-norm.md) obeys the [energy estimate](../../../../../../energy-estimate.md)

$$
\frac12\frac d{dt}\int_{-1}^1w^2\,dx
=-\int_{-1}^1w_x^2\,dx+\frac a2[w^2]_{-1}^1+\int_{-1}^1bw^2\,dx\leq0.
$$

The boundary term vanishes and $b\leq0$. A nonnegative quantity starting at zero must stay zero, proving uniqueness in the usual classical or corresponding energy class.

The printed evenness claim for $a=0$ is **false for an arbitrary coefficient $b(x,t)\leq0$**. Take $T_0>0$ and $b(x,t)=-2-x$. The [strong maximum principle](../../../../../../strong-maximum-principle-for-elliptic-operators.md) makes the solution positive in the interior for $t>0$. If it were even, $T_t$ and $T_{xx}$ would both be even. Subtracting the equation at $x$ and $-x$ would give $0=[b(x,t)-b(-x,t)]T(x,t)=-2xT(x,t)$, impossible for $x\ne0$.

With the additional assumption $b(-x,t)=b(x,t)$, the intended argument is valid. For $a=0$, [reflection](../../../../../../reflection-mathematics.md) $\widetilde T(x,t)=T(-x,t)$ solves the same equation with the same initial and boundary data. Uniqueness then proves $\boxed{T(-x,t)=T(x,t)}$. If $T_0\ne0$, initial and boundary values disagree at the two time-zero corners; the [initial condition](../../../../../../initial-condition.md) is understood in the interior or in the [L2 norm](../../../../../../l2-norm.md) [limit](../../../../../../limit-of-a-function.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [6](../../6.md)
3. [Mathematics V](../../../mathematics-v-split.md)
4. [Prelims](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
