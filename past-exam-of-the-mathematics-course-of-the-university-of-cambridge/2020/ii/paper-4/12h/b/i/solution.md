<h1 id="12h/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The convergents satisfy

$$
p_nq_{n-1}-p_{n-1}q_n=(-1)^{n-1},
$$

so $(p_n,q_n)$ and $(p_{n-1},q_{n-1})$ form an integer basis of $\mathbb Z^2$. Put $\delta_j=q_j\alpha-p_j$. Consecutive errors have opposite signs and $|\delta_{n-1}|>|\delta_n|$.

For integers $p,q$ with $0<q\leq q_n$, write

$$
(p,q)=r(p_n,q_n)+s(p_{n-1},q_{n-1}).
$$

If $s>0$, the denominator bound forces $r\leq0$, while if $s<0$ positivity forces $r\geq1$. Because $\delta_n$ and $\delta_{n-1}$ have opposite signs, in either case $s\neq0$ implies

$$
|q\alpha-p|=|r\delta_n+s\delta_{n-1}|>|\delta_n|.
$$

If $s=0$, the denominator bound gives $r=1$ unless the fraction is zero or has the same value as $p_n/q_n$. Thus $p_n/q_n$ is a [best approximation of the second kind](../../../../../../../best-approximation-of-the-second-kind.md). Dividing by $q\leq q_n$ gives

$$
\boxed{\left|\alpha-\frac pq\right|
=\frac{|q\alpha-p|}{q}
\geq\frac{|q_n\alpha-p_n|}{q_n}
=\left|\alpha-\frac{p_n}{q_n}\right|.}
$$

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [12H](../../../12h.md)
4. [Paper 4](../../../../paper-4-split.md)
5. [Ii](../../../../split.md)
6. [2020](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
