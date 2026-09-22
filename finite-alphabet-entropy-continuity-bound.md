# Finite-alphabet entropy continuity bound

↑ **Parent:** [Information entropy](information-entropy-split.md)

For [probability mass functions](probability-mass-function.md) on $N$ symbols, set $d_i=|p_i-q_i|$ and $d=\sum_id_i\leq1/2$. The [entropy summand](entropy-summand.md) bound gives $|f(p_i)-f(q_i)|\leq f(d_i)$. The [triangle inequality](triangle-inequality.md) and [Jensen's inequality](jensen-s-inequality.md) give

$$
|H(p)-H(q)|\leq\sum_if(d_i)\leq Nf(d/N)=d\log_2(N/d).
$$

At $d=0$, use the continuous value zero. This proves uniform continuity of [Shannon entropy](information-entropy-split.md) on a fixed [finite alphabet](finite-alphabet.md); the [alphabet](alphabet.md) size appears explicitly in the bound.

## ↑ Ancestors (6)

1. [Information entropy](information-entropy-split.md)
2. [Information theory](information-theory-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-information-theory-course-of-the-university-of-oxford/2023/1/d/solution.md)
