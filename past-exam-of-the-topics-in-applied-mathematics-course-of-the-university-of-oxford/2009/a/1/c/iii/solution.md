<h1 id="a/1/c/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Let $L=\log r$. The given expansion implies $u_*=2L+O(L/r)$ and therefore

$$
e^{-u_*}=r^{-2}[1+O(L/r)].
$$

Using $H'(u)=re^{-u}(1-u)$ gives precisely

$$
\boxed{H'(u_*)=\frac1r[1-2L+O(L/r)][1+O(L/r)].}
$$

The paired low value is $v_*=H(u_*)=(2L/r)[1+O(L/r)]$. It is small, so $e^{-v_*}(1-v_*)=1+O(L/r)$ and

$$
\boxed{H'(H(u_*))=r[1+O(L/r)]\sim r.}
$$

By the [chain rule](../../../../../../chain-rule.md) the second-iterate [periodic-orbit multiplier](../../../../../../multiplier-of-a-periodic-orbit-of-an-iteration.md) is their product:

$$
(H^2)'(u_*)=1-2L+O(L^2/r).
$$

Since $L^2/r\to0$ while $L\to\infty$, this tends to $-\infty$ and eventually has magnitude above one. Thus **the large second-iterate [fixed point](../../../../../../fixed-point.md), and hence its associated [two-cycle](../../../../../../period-two-orbit.md), is unstable for sufficiently large $r$**. The high state's small [derivative](../../../../../../derivative.md) alone does not imply stability: the low state's [derivative](../../../../../../derivative.md) supplies the compensating factor of order $r$.

## ↑ Ancestors (14)

1. [Iii](../iii.md)
2. [C](../../c.md)
3. [1](../../../1.md)
4. [A](../../../../a.md)
5. [2009](../../../../../2009-split.md)
6. [Past exam of the topics in applied mathematics course of the University of Oxford](../../../../../split.md)
7. [Topics in applied mathematics course of the University of Oxford](../../../../../../topics-in-applied-mathematics-course-of-the-university-of-oxford.md)
8. [Year 3 of the mathematics course of the University of Oxford](../../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
