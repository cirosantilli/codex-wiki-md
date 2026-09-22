<h1 id="6/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Write $f^{(4)}(x)=24(5-4x)/x^6$. Its [derivative](../../../../../derivative.md) is $f^{(5)}(x)=240(2x-3)/x^7$, so on $[1,2]$ it decreases to $x=3/2$ and then increases. Its endpoint and turning-point values are

$$
f^{(4)}(1)=24,\qquad
f^{(4)}(3/2)=-\frac{512}{243},\qquad
f^{(4)}(2)=-\frac98.
$$

Thus $M_4=24$, and the preceding bound becomes

$$
\boxed{|I-S_n|\leq\frac{2}{15n^4}\qquad(n\text{ even}).}
$$

For the [rounding](../../../../../rounding.md) estimate, standard binary64 has spacing $\epsilon=2^{-52}$ above one. Balancing this nominal absolute accuracy with the bound gives

$$
n\approx\left(\frac{2}{15\epsilon}\right)^{1/4}\approx4.95\times10^3.
$$

Thus **a few thousand even strips, roughly $5000$, reach the double-precision scale according to this bound**. A scale-aware estimate leads to the same order. Indeed,

$$
I=-\frac{19}{6}-4\log2\approx-5.9392553889
$$

lies in magnitude between $4$ and $8$, where the binary64 spacing is $2^{-50}$. Balancing the error bound against half that spacing gives about $4.16\times10^3$ strips.

These are saturation estimates from [balancing quadrature truncation and round-off error](../../../../../balancing-quadrature-truncation-and-round-off-error.md), not sharp guarantees of the actual [rounding](../../../../../rounding.md) plateau. The error bound can be conservative, and evaluation and summation errors can limit accuracy earlier. Merely storing the final result does not specify every source of [rounding error](../../../../../round-off-error.md).

## ↑ Ancestors (12)

1. [D](../d.md)
2. [6](../../6.md)
3. [Discrete mathematics, continuous mathematics and probability resit](../../../discrete-mathematics-continuous-mathematics-and-probability-resit-split.md)
4. [2022](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
