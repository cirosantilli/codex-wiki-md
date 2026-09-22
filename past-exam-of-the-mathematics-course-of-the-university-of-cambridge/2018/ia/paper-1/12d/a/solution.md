<h1 id="12d/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Assume $a_n\to0$. The function is bounded, and every interval has lower [Darboux sum](../../../../../../darboux-sum.md) zero because it contains an irrational. Given $\varepsilon>0$, choose $N$ so that $a_n<\varepsilon/2$ for $n>N$. Put small intervals around the finitely many points $q_1,\ldots,q_N$ whose total length makes their contribution to the upper sum less than $\varepsilon/2$, and refine their endpoints to a partition. On every remaining subinterval the function is at most $\varepsilon/2$, so the upper sum is less than $\varepsilon$. The [Riemann integrability criterion](../../../../../../riemann-integrability-criterion.md) proves that **$f$ is Riemann integrable with integral zero**.

The condition $a_n\to0$ is sufficient but not necessary. Assign $a_n=1$ when $q_n=1/k$ for some positive integer $k$, and $a_n=1/n$ otherwise. Then $(a_n)$ does not tend to zero. Outside a short interval near zero only finitely many unit spikes occur and can be enclosed in intervals of arbitrarily small total length; all remaining values can be made uniformly small except for finitely many further points. The same Darboux-sum argument proves that this $f$ is Riemann integrable with integral zero.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [12D](../../12d.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
