<h1 id="5/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

On $I=[1,7/5]$, $f'<0$ and $f''<0$, since $x^2<2$. Hence $|f'|$ increases and has minimum $|f'(1)|=14$. Also

$$
|f''(x)|=30x^2(2-x^2)
=30\bigl(1-(x^2-1)^2\bigr)\le30,
$$

with equality at $x=1$. Therefore

$$
\boxed{\frac{\max_I|f''|}{\min_I|f'|}=\frac{30}{14}=\frac{15}{7}.}
$$

There is a unique root $r$ in $I$: $f(1)=2>0$, $f(7/5)=-5.678464<0$, and the [function](../../../../../../function-split.md) is strictly decreasing. Moreover $f(6/5)=-1.382016<0$, so $r<6/5=x_0$.

It remains to justify that the iteration stays where the error estimate applies. Because $f$ is a [concave function](../../../../../../concave-function.md), its graph lies below each [tangent line](../../../../../../tangent-line.md). At any $x\in[r,6/5]$, the tangent has nonpositive value $f(x)$ at $x$, negative slope, and nonnegative value at $r$. Its zero $N(x)=x-f(x)/f'(x)$ therefore satisfies

$$
r\le N(x)\le x.
$$

By [mathematical induction](../../../../../../mathematical-induction.md), the [Newton root-finding iteration](../../../../../../newton-root-finding-iteration.md) stays in $[r,6/5]$ and decreases to some limit $L\ge r$. Continuity in $x_{k+1}-x_k=-f(x_k)/f'(x_k)$ implies $f(L)=0$, so uniqueness gives $L=r$.

Now the supplied error bound applies at every step:

$$
\boxed{|x_{k+1}-r|\le\frac{15}{14}|x_k-r|^2.}
$$

This proves at least [quadratic convergence](../../../../../../quadratic-convergence.md), with an invariant [interval](../../../../../../interval-mathematics.md) and a nonvanishing [derivative](../../../../../../derivative.md) explicitly established.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [5](../../../5.md)
4. [Discrete mathematics, continuous mathematics, and probability](../../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
5. [2019](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
