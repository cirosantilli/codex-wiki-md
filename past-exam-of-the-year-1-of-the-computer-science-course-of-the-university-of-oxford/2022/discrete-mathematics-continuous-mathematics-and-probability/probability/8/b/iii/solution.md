<h1 id="probability/8/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The extra ancestor multiplies the [probability generating function](../../../../../../../probability-generating-function.md) by $s$. The preceding [probability generating function of an independent random sum](../../../../../../../probability-generating-function-of-an-independent-random-sum.md) formula therefore yields

$$
G_Z(s)=sG_N(G_Z(s))=\frac{s}{2-G_Z(s)},\qquad G_Z(s)^2-2G_Z(s)+s=0.
$$

For $0\le s<1$ the two roots are $1\pm\sqrt{1-s}$. A [probability generating function](../../../../../../../probability-generating-function.md) lies in $[0,1]$ there, so the plus root is impossible. Also $Z\ge1$ gives $G_Z(0)=0$. Consequently the [total progeny with critical geometric offspring](../../../../../../../total-progeny-with-critical-geometric-offspring.md) has

$$
\boxed{G_Z(s)=1-\sqrt{1-s},\qquad 0\le s\le1.}
$$

At $s=1$ the value is $1$, consistent with almost-sure finiteness. For complex $|s|<1$, the same expression uses the analytic square root that equals $1$ at $s=0$.

## ↑ Ancestors (14)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [8](../../../8.md)
4. [Probability](../../../../probability.md)
5. [Discrete mathematics, continuous mathematics, and probability](../../../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
6. [2022](../../../../../split.md)
7. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../../split.md)
8. [Year 1 of the computer science course of the University of Oxford](../../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
9. [Computer science course of the University of Oxford](../../../../../../../computer-science-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../../split.md)
