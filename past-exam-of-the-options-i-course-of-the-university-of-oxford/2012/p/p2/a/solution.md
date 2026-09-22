<h1 id="p/p2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The leading error term can be removed by comparing the two step sizes $h$ and $h/2$:

$$
I_h=I-K_2h^2-K_4h^4-\cdots,\qquad
I_{h/2}=I-\frac14K_2h^2-\frac1{16}K_4h^4-\cdots.
$$

Multiply the second expression by four and subtract the first. The $h^2$ terms cancel, so the first [Richardson extrapolation](../../../../../richardson-extrapolation.md) step is

$$
\boxed{R_1(h)=\frac{4I_{h/2}-I_h}{3},\qquad I-R_1(h)=-\frac14K_4h^4+O(h^6).}
$$

Repeat with $R_1(h/2)$ and $R_1(h)$, now cancelling the fourth-order error using the factor $16$. In general, with $R_0(h)=I_h$,

$$
\boxed{R_j(h)=\frac{4^jR_{j-1}(h/2)-R_{j-1}(h)}{4^j-1}.}
$$

Under the stated even-power expansion, successive columns have errors of orders $h^4,h^6,h^8,\ldots$. Each step uses the known scaling of the leading error to eliminate its unknown coefficient.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [P2](../../p2.md)
3. [P](../../../p.md)
4. [2012](../../../../2012-split.md)
5. [Past exam of the options I course of the University of Oxford](../../../../split.md)
6. [Options I course of the University of Oxford](../../../../../options-i-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
