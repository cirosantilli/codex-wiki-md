<h1 id="5/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

A small difference between successive [secant method](../../../../../../secant-method.md) iterates alone does not certify a small absolute error. Instead use a [residual root error bound](../../../../../../residual-root-error-bound.md). On $[2,3]$,

$$
f'(x)=\frac{\ln x+1}{\ln2}\geq m:=1+\frac1{\ln2}>0,
$$

and $f(2)<0<f(3)$, so there is a unique [root](../../../../../../root-of-a-root-system.md) $r\in(2,3)$. For an iterate $x\in[2,3]$, the [mean value theorem](../../../../../../mean-value-theorem.md) gives

$$
|x-r|=\frac{|f(x)|}{|f'(\xi)|}\leq\frac{|f(x)|}{m}.
$$

Therefore **stop when $x\in[2,3]$ and $|x\log_2x-4|\leq(1+1/\ln2)10^{-10}$**. This guarantees the desired absolute error in exact arithmetic; the evaluated [residual of a root equation](../../../../../../residual-of-a-root-equation.md) should include an allowance for its much smaller [roundoff error](../../../../../../round-off-error.md). A safeguarded implementation can retain the bracket $[2,3]$ and use [bisection](../../../../../../bisection-method.md) if a proposed [secant method](../../../../../../secant-method.md) step leaves it.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [5](../../../5.md)
4. [Discrete mathematics, continuous mathematics, and probability resit](../../../../discrete-mathematics-continuous-mathematics-and-probability-resit-split.md)
5. [2019](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
