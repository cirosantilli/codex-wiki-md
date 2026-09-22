<h1 id="3/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Substitute a [Frobenius series](../../../../../frobenius-solution.md) $y=\sum_{n\geq0}a_nz^{n+\rho}$ into the transformed equation. For $n\geq1$, equating the coefficient of $z^{n+\rho-1}$ gives the [recurrence relation](../../../../../recurrence-relation.md)

$$
(n+\rho)(n+\rho-2)a_n+(n+\rho-1+c)a_{n-1}=0.
$$

At the larger [indicial root](../../../../../indicial-root.md) $\rho=2$, the coefficient of $a_n$ is $n(n+2)\ne0$, so a [Frobenius solution](../../../../../frobenius-solution.md) always exists. At the smaller [indicial root](../../../../../indicial-root.md) $\rho=0$, the first two equations are

$$
a_1=ca_0,\qquad0\cdot a_2+(1+c)a_1=0.
$$

Since $a_0\ne0$, the exceptional equation is consistent exactly when

$$
\boxed{c(c+1)=0,\qquad c=0\ \text{or}\ c=-1.}
$$

These are **both admissible values**, including the zero value; the singular wording of the question does not remove either. This is the [undetermined coefficient at Frobenius resonance](../../../../../undetermined-coefficient-at-frobenius-resonance.md): at either value $a_2$ is free, whereas otherwise the second independent solution requires a [Logarithmic Frobenius solution](../../../../../logarithmic-solution-from-a-repeated-frobenius-exponent.md).

Explicit pairs demonstrate sufficiency and [linear independence](../../../../../linear-independence.md). In the variable $z=x+1$ one may take

$$
\begin{array}{c|cc}
c&u_0(z)&u_2(z)\\\hline
0&1&1-(1+z)e^{-z}\\
-1&1-z&e^{-z}+z-1.
\end{array}
$$

Both displayed $u_2$ have leading term $z^2/2$, while $u_0(0)=1$. They therefore give independent [Frobenius solutions](../../../../../frobenius-solution.md) with the two [indicial exponents](../../../../../indicial-exponent.md), and direct [differentiation](../../../../../differentiation.md) verifies the equation. The point is an [apparent regular singular point](../../../../../apparent-regular-singular-point.md) in these two cases.

For the requested closed forms, particularly short choices are

$$
\boxed{y(x)=1\quad(c=0),\qquad y(x)=x\quad(c=-1).}
$$

In addition, $(x+2)e^{-x}$ solves the zero-parameter equation and $e^{-x}$ solves the equation with $c=-1$.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [3](../../../3.md)
4. [2017](../../../../2017-split.md)
5. [Past exam of the differential equations 2 course of the University of Oxford](../../../../split.md)
6. [Differential equations 2 course of the University of Oxford](../../../../../differential-equations-2-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
