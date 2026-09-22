<h1 id="6/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Here a dense $100000$-by-$100000$ [matrix](../../../../../../matrix.md) has $10^{10}$ entries, about $80$ GB even with eight-byte storage per entry. Use [limited-memory BFGS](../../../../../../limited-memory-bfgs.md) on the negative of the objective, or equivalently its positive-definite approximate-metric form of [gradient ascent](../../../../../../gradient-ascent.md). It stores only a fixed small number $\ell$ of [vector](../../../../../../vector.md) pairs, costing $O(\ell d)$ memory rather than $O(d^2)$.

Let $G(x)=\sum_{i=1}^{100}e^{e^{-\|x-a_i\|^2}}$ and put $c_i(x)=e^{e^{-\|x-a_i\|^2}}e^{-\|x-a_i\|^2}$. Direct use of the [chain rule](../../../../../../chain-rule.md) gives

$$
\nabla G(x)=-2\sum_{i=1}^{100}c_i(x)(x-a_i).
$$

If $H_n$ denotes the positive-definite inverse-[Hessian matrix](../../../../../../hessian-matrix.md) approximation for $-G$, the iteration is

$$
x_{n+1}=x_n+\alpha_nH_n\nabla G(x_n),
$$

with a [line search](../../../../../../line-search.md) increasing $G$ and the usual safeguarded limited-memory updates. No exact [Hessian matrix](../../../../../../hessian-matrix.md) is required. With fixed memory and the usual bounded-metric and [line search](../../../../../../line-search.md) hypotheses, expect **local [linear convergence](../../../../../../linear-convergence.md) near a nondegenerate strict maximum**; fixed-memory [limited-memory BFGS](../../../../../../limited-memory-bfgs.md) does not generally inherit the superlinear theorem for full-memory [BFGS](../../../../../../bfgs-method.md).

Unlike the preceding objective, $G$ is not generally a [concave function](../../../../../../concave-function.md). Thus this is a method for finding a [local maximum](../../../../../../local-maximum.md); comparison of different converged candidates or a global search is needed to certify a [global maximum](../../../../../../global-maximum.md) for arbitrary centres. The symbolic problem supplies no assumption that would justify an unconditional global-convergence claim.[Final paragraphs: storing only recent secant [vectors](../../../../../../vector.md), linear-in-dimension memory, and the L-BFGS implementation](../../../../../../quasi-newton-methods-by-neos-guide.md)

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [6](../../../6.md)
4. [Discrete mathematics, continuous mathematics, and probability](../../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
5. [2021](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
