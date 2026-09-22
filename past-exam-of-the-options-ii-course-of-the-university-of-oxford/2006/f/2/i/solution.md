<h1 id="f/2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [Fréchet derivative](../../../../../frechet-derivative.md) at $a$ is the [linear map](../../../../../linear-map.md) $Df_a:\mathbb R^n\to\mathbb R^k$ satisfying

$$
f(a+h)=f(a)+Df_a(h)+r(h),\qquad
\frac{\|r(h)\|}{\|h\|}\longrightarrow0.
$$

It is unique. When both derivatives exist, the [chain rule](../../../../../chain-rule.md) is $D(g\circ f)_a=Dg_{f(a)}\circ Df_a$.

For the square map,

$$
(A+\Delta)^2-A^2=A\Delta+\Delta A+\Delta^2.
$$

The remainder has norm at most $\|\Delta\|^2$ in a submultiplicative [matrix norm](../../../../../matrix-norm.md), hence is $o(\|\Delta\|)$. Therefore

$$
\boxed{DS_A(\Delta)=A\Delta+\Delta A.}
$$

[Matrix](../../../../../matrix.md) multiplication is not commutative, so the two terms cannot generally be combined as $2A\Delta$.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [2](../../2.md)
3. [F](../../../f.md)
4. [2006](../../../../2006-split.md)
5. [Past exam of the options II course of the University of Oxford](../../../../split.md)
6. [Options II course of the University of Oxford](../../../../../options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
