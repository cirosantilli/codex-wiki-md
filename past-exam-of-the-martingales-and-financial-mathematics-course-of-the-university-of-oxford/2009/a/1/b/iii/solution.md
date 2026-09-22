<h1 id="a/1/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Suppose first that [complete convergence](../../../../../../complete-convergence-of-random-variables.md) holds. For each positive integer $j$, apply the [First Borel-Cantelli lemma](../../../../../../borel-cantelli-first-lemma.md) to $\{|X_n-X|>1/j\}$. Outside a countable union of null events, only finitely many of these exceedances occur for every $j$. This is [almost sure convergence](../../../../../../almost-sure-convergence.md), with no independence assumption.

For the converse, an important point is that independence of $X_n$ does not immediately imply independence of $X_n-X$. Instead use the fact that an [almost-sure limit of independent random variables is constant](../../../../../../almost-sure-limit-of-independent-random-variables-is-constant.md). Indeed, $Z=\limsup_nX_n$ is measurable for the [tail sigma-algebra](../../../../../../tail-sigma-algebra.md). The [Kolmogorov zero-one law](../../../../../../kolmogorov-s-zero-one-law.md) makes each event $\{Z\leq q\}$, $q\in\mathbb Q$, have probability zero or one. Since $Z=X$ almost surely and $X$ is finite, these probabilities form the distribution function of a point mass: there is a finite constant $c$ with $X=c$ almost surely.

Now $\{|X_n-c|>\epsilon\}$ are independent events. [Almost sure convergence](../../../../../../almost-sure-convergence.md) says that their infinitely-often event has probability zero. The contrapositive of the [Second Borel-Cantelli lemma](../../../../../../borel-cantelli-second-lemma.md) gives

$$
\sum_n\mathbb P(|X_n-c|>\epsilon)<\infty.
$$

Replacing $c$ by the almost surely equal $X$ leaves each probability unchanged. Thus **complete convergence and almost sure convergence are equivalent for independent sequences**.

## ↑ Ancestors (14)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [1](../../../1.md)
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
