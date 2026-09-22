<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the stated characterization by the [Lq null space property](../../../../../../lq-null-space-property.md). Raising an [Lq quasi-norm](../../../../../../lq-quasi-norm.md) comparison to its positive exponent preserves its order, so the hypothesis at $q$ says that, for every nonzero $v\in\ker A$ and every $|S|\le s$,

$$
\sum_{j\in S}|v_j|^q<\sum_{j\notin S}|v_j|^q.
$$

We prove the corresponding $p$ inequality; this is [monotonicity of uniform sparse recovery in the exponent](../../../../../../monotonicity-of-uniform-sparse-recovery-in-the-exponent.md).

Fix a nonzero [null space](../../../../../../kernel-of-a-linear-map.md) [vector](../../../../../../vector.md) and arrange its coordinate magnitudes as $a_1\ge\cdots\ge a_N\ge0$. Assume $s\ge1$. The [Lq null space property](../../../../../../lq-null-space-property.md) rules out a nonzero [null space](../../../../../../kernel-of-a-linear-map.md) [vector](../../../../../../vector.md) supported on at most $s$ coordinates, so $s<N$ and $t=a_s>0$. Since $p-q<0$, the factors $a_j^{p-q}$ are at most $t^{p-q}$ for $j\le s$ and at least $t^{p-q}$ for $j>s$ with $a_j>0$. Terms with $a_j=0$ contribute zero and require no negative power of zero. Thus

$$
\sum_{j=1}^s a_j^p\le t^{p-q}\sum_{j=1}^s a_j^q<t^{p-q}\sum_{j=s+1}^N a_j^q\le\sum_{j=s+1}^N a_j^p.
$$

The largest $s$ coordinates maximize the $p$-power sum on any set of size at most $s$. Its complement therefore has the smallest complementary $p$-power sum. The displayed strict inequality proves the [Lq null space property](../../../../../../lq-null-space-property.md) at exponent $p$ for every allowed [support of a vector](../../../../../../support-of-a-vector.md). The stated recovery characterization now applies to the [Lq quasi-norm](../../../../../../lq-quasi-norm.md) at $p$.

If $\ker A=\{0\}$, the measurement constraint already singles out $x$, for every objective; if $s=0$, only the zero [sparse vector](../../../../../../sparse-vector.md) needs recovery. These cases do not need a positive threshold. **Uniform recovery at $q$ implies uniform recovery at every $0<p<q$:**

$$
\boxed{q\text{-recovery of order }s\ \Longrightarrow\ p\text{-recovery of order }s.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
