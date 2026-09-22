<h1 id="6/c/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

**At $d=10^6$, [gradient descent](../../../../../../gradient-descent-split.md) remains a plausible large-scale choice; dense [Newton method](../../../../../../newton-s-method-in-optimization.md) and full-memory [BFGS](../../../../../../bfgs-method.md) are generally impractical.** A dense $d\times d$ double-precision [matrix](../../../../../../matrix.md) alone contains $10^{12}$ entries, about $8$ TB. Dense factorization also has order $10^{18}$ arithmetic work. Full [BFGS](../../../../../../bfgs-method.md) avoids factorization but retains quadratic storage and update work, so it does not solve that scaling problem.

[Gradient descent](../../../../../../gradient-descent-split.md) uses linear working storage in $d$, though the cost of reading the data and evaluating the [gradient](../../../../../../gradient.md) is still $O(nd)$ for dense $A$. Sparsity or streaming can be important. [Limited-memory BFGS](../../../../../../limited-memory-bfgs.md), a distinct limited-memory variant, stores only a fixed number $m$ of recent update pairs and uses $O(md)$ storage and update work, making it a realistic alternative to full [BFGS](../../../../../../bfgs-method.md).[Final paragraphs: implicit inverse-Hessian products and stored-pair limited-memory methods](../../../../../../quasi-newton-methods-by-neos-guide.md)

The available [Hessian matrix](../../../../../../hessian-matrix.md) factorization also permits a [matrix-free Hessian-vector product](../../../../../../matrix-free-hessian-vector-product.md):

$$
Hv=A^{\mathsf T}\bigl(\Delta(Av)\bigr).
$$

It costs $O(nd)$ for dense data without forming $H$. A suitable iterative, safeguarded [Newton method](../../../../../../newton-s-method-in-optimization.md) can exploit this structure, so the conclusion rules out the dense implementation rather than every possible second-order algorithm.

These methods seek a local solution and require convergence checks appropriate to nonconvex [optimization](../../../../../../mathematical-optimization-split.md). The formula does not even ensure a finite minimizer exists: with one positive coefficient and nonzero $\mathbf a$, the positive exponential loss approaches zero along an unbounded direction without attaining it. Dimension alone cannot supply a convergence guarantee.

## ↑ Ancestors (13)

1. [Iv](../iv.md)
2. [C](../../c.md)
3. [6](../../../6.md)
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
