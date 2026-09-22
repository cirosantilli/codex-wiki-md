<h1 id="4f/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $E_\ell$ be the event that the block beginning at position $\ell$, $1\leq\ell\leq k+1$, is a spalindrome. Each has probability $(10)_k/10^{2k}$. If two starting positions differ by $d<k$, the first half of the later block contains the middle digit of the earlier palindrome twice, contradicting distinctness. Thus the only possible overlap is $E_1\cap E_{k+1}$.

That intersection consists of words $A\,A^{\rm rev}A$, where $A$ has $k$ distinct digits, and hence has probability $(10)_k/10^{3k}$. This [overlap structure of digit spalindromes](../../../../../../overlap-structure-of-digit-spalindromes.md) makes inclusion--exclusion give

$$
\boxed{\mathbb P\left(\bigcup_{\ell=1}^{k+1}E_\ell\right)
=(k+1)\frac{(10)_k}{10^{2k}}
-\frac{(10)_k}{10^{3k}}.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4F](../../4f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
