<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Replace the same last $k$ vectors by $(100,\ldots,100)$. Applying part a to each independent Gaussian coordinate shows that the probability its contaminated coordinate median exceeds $\epsilon$ is at least $1-e^{-c_\epsilon n}$. Independence across coordinates and [Bernoulli's inequality](../../../../../../bernoulli-s-inequality.md) give

$$
\mathbb P\!\left(
\widehat\mu_j>\epsilon\text{ for every }j
\right)
\geq(1-e^{-c_\epsilon n})^d
\geq1-de^{-c_\epsilon n}.
$$

For $n$ sufficiently large as a function of $d$ and $\epsilon$, the last expression is at least $1/2$. On this event,

$$
\|\widehat\mu\|_2>\epsilon\sqrt d,
$$

which proves the stated lower bound for the supremum over adversarial perturbations.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 223](../../../paper-223-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
