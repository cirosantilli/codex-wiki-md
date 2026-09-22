<h1 id="26j/solution">Solution</h1>

↑ **Parent:** [26J](../26j.md)

A [simple function](../../../../../simple-function.md) is a measurable function with finitely many values, written $s=\sum_{j=1}^m a_j\mathbf1_{A_j}$ using disjoint measurable sets. For nonnegative $s$ its [Lebesgue integral](../../../../../lebesgue-integral.md) is $\mu(s)=\sum_ja_j\mu(A_j)$, with $0\cdot\infty=0$. An integrable signed simple function has $\sum_j|a_j|\mu(A_j)<\infty$ and the same signed sum defines its integral.

For a nonnegative measurable $f$ define $\mu(f)=\sup\{\mu(s):s\text{ simple},\ 0\leq s\leq f\}$. A real measurable $f$ is [Lebesgue integrable](../../../../../lebesgue-integrable-function.md) when $\mu(|f|)<\infty$; then $\mu(f)=\mu(f^+)-\mu(f^-)$, both terms finite. The [monotone convergence theorem](../../../../../monotone-convergence-theorem.md) states that if $0\leq f_n\uparrow f$ pointwise, or almost everywhere, then $\mu(f_n)\uparrow\mu(f)$, allowing infinity.

For nonnegative $f,g$, choose nonnegative simple approximations $s_n\uparrow f$, $t_n\uparrow g$. Their sums increase to $f+g$; simple-function additivity and [monotone convergence](../../../../../monotone-convergence-theorem.md) give $\mu(f+g)=\mu(f)+\mu(g)$. The same approximation proves $\mu(cf)=c\mu(f)$ for $c\geq0$.

For integrable signed $f,g$, $|f+g|\leq|f|+|g|$ makes their sum integrable. Write $u=f^++g^+$, $v=f^-+g^-$. The identity $u+(f+g)^-=v+(f+g)^+$ and nonnegative additivity, with finite integrals, give $\mu(f+g)=\mu(f)+\mu(g)$. Also $(cf)^\pm=c f^\pm$ when $c\geq0$, while negative $c$ interchanges the two parts, so $\mu(cf)=c\mu(f)$ for every real $c$. Integrals do not change upon alteration on a null set, hence this descends to [Lebesgue space](../../../../../lp-space.md). **The indicated map is linear.**

## ↑ Ancestors (10)

1. [26J](../26j.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
