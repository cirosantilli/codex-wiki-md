<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Apply the [mean value theorem](../../../../../mean-value-theorem.md), the first-order case of [Taylor's theorem](../../../../../taylor-s-theorem.md), to $f'$ between $0$ and $x>1$. It yields

$$
f'(x)=3+xf''(\xi)\geq3+2x>5.
$$

Also $f(3/2)\geq-5+9/2+9/4=7/4>0$, so the initial point is to the right of the root $x^*$. For an increasing [strictly convex function](../../../../../strictly-convex-function.md), its tangent at a point to the right of a root meets the axis between that root and the point. Hence the exact [Newton root-finding iteration](../../../../../newton-root-finding-iteration.md) remains in $[x^*,3/2]$ and decreases towards $x^*$.

On every relevant [interval](../../../../../interval-mathematics.md), $|f''|<3$ and $f'>5$, so the stated [quadratic convergence](../../../../../quadratic-convergence.md) bound gives, with $e_n=|x_n-x^*|$,

$$
e_{n+1}\leq\tfrac3{10}e_n^2,\qquad e_0<\tfrac12.
$$

Iterating the bound gives

$$
e_1<0.075,\quad e_2<0.0016875,\quad
 e_3<8.543\times10^{-7},\quad e_4<2.190\times10^{-13}<2^{-40}.
$$

Thus **four Newton corrections suffice to reduce the exact-iteration error bound below the floating-point spacing scale**. The [quadratic convergence](../../../../../quadratic-convergence.md) doubles the approximate number of correct digits at each late step. Beyond this point further corrections cannot reliably improve a generic floating-point answer. This is a bound on useful accuracy under the usual stable-evaluation model, not a claim that the data specify the exact iteration at which every implementation must stagnate.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [4](../../4.md)
3. [Discrete mathematics, continuous mathematics, and probability](../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
4. [2021](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
