<h1 id="5/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

At $x=0$, $f_n(x)=0$. For fixed $x>0$,

$$
0\leq f_n(x)=\frac{nx}{1+n^2x^2}\leq\frac1{nx}\longrightarrow0.
$$

Thus the [pointwise limit](../../../../../../../pointwise-limit.md) is zero everywhere on $[0,1]$. However, with $t=nx$, the inequality $1+t^2\geq2t$ gives $f_n(x)\leq1/2$, and equality occurs at $x=1/n\in[0,1]$. Hence

$$
\boxed{\|f_n\|_\infty=\frac12\quad\text{for every }n\geq1,}
$$

so there is **no [uniform convergence](../../../../../../../uniform-convergence.md)**. The moving evaluation point $1/n$ captures a peak missed by each fixed positive input.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [C](../../c.md)
3. [5](../../../5.md)
4. [Mathematics II](../../../../mathematics-ii-split.md)
5. [Prelims](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
