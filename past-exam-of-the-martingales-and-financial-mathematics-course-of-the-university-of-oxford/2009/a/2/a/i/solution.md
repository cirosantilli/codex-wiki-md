<h1 id="a/2/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

A real-valued [random variable](../../../../../../random-variable-split.md) is a [measurable function](../../../../../../measurable-function.md) $Y:(\Omega,\mathcal F)\to(\mathbb R,\mathcal B(\mathbb R))$: equivalently, $\{Y\leq t\}\in\mathcal F$ for every real $t$.

For $p=1$ the asserted inequality is equality. For $p>1$, let $q=p/(p-1)$. If $\mathbb E Y^p=\infty$, the inequality is automatic. Otherwise [Hölder's inequality](../../../../../../holder-s-inequality.md) on the probability space gives

$$
\mathbb E Y=\mathbb E(Y\cdot1)\leq(\mathbb E Y^p)^{1/p}(\mathbb E1^q)^{1/q}
=(\mathbb E Y^p)^{1/p}.
$$

Thus $\boxed{\|Y\|_1\leq\|Y\|_p}$, using that the total measure is one.

## ↑ Ancestors (14)

1. [I](../i.md)
2. [A](../../a.md)
3. [2](../../../2.md)
4. [A](../../../../a.md)
5. [2009](../../../../../2009-split.md)
6. [Past exam of the martingales and financial mathematics course of the University of Oxford](../../../../../split.md)
7. [Martingales and financial mathematics course of the University of Oxford](../../../../../../martingales-and-financial-mathematics-course-of-the-university-of-oxford.md)
8. [Year 3 of the mathematics course of the University of Oxford](../../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
