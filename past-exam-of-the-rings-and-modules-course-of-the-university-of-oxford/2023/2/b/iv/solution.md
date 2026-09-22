<h1 id="2/b/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

For every $i\in\mathbb N_0$, truncate $w$ before coordinate $i$:

$$
f_i(j)=\begin{cases}w(j),&j<i,\\0,&j\geq i.\end{cases}
$$

This $f_i$ lies in $F$. For $j<i$, $(w-f_i)(j)=0$. For $j\geq i$, $(w-f_i)(j)=w(j)=\pm2^j$, which is divisible by $2^i$. In particular the integer sequence

$$
g_i(j)=\begin{cases}0,&j<i,\\w(j)/2^i,&j\geq i\end{cases}
$$

belongs to $B$ and satisfies $w=f_i+2^ig_i$.

Apply the [module homomorphism](../../../../../module-homomorphism.md) $\pi$. Since $f_i\in F\subseteq\ker\pi$,

$$
\pi(w)=2^i\pi(g_i)\qquad\text{for every }i\in\mathbb N_0.
$$

Fixing any coordinate $j$, the [integer](../../../../../integer-split.md) $\pi(w)(j)$ is therefore divisible by $2^i$ for every $i$. The only such [integer](../../../../../integer-split.md) is zero: if $a\ne0$, choose $i$ with $2^i>|a|$, which rules out $a=2^ib$ for any nonzero [integer](../../../../../integer-split.md) $b$. Thus every coordinate of $\pi(w)$ vanishes, contradicting part (b)(iii).

It follows that

$$
\boxed{B=\prod_{j\in\mathbb N_0}\mathbb Z\text{ is not a free }\mathbb Z\text{-module}}.
$$

The decisive property is [vanishing of infinitely divisible integer sequences](../../../../../vanishing-of-infinitely-divisible-integer-sequences.md), namely $\bigcap_{i\geq0}2^iB=\{0\}$.

## ↑ Ancestors (13)

1. [Iv](../iv.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the rings and modules course of the University of Oxford](../../../../split.md)
6. [Rings and modules course of the University of Oxford](../../../../../rings-and-modules-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
