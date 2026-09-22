<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Set $h(O_E)=0$ and

$$
h(P)=\log H(x(P))
$$

for $P\ne O_E$. The [canonical height of an elliptic curve](../../../../../../canonical-height-of-an-elliptic-curve.md) is

$$
\widehat h(P)=\frac12\lim_{r\to\infty}4^{-r}h([2^r]P).
$$

The duplication formula is a rational function of degree four in $x$, so the rational-map height estimate in part (a) gives

$$
|h([2]P)-4h(P)|\leq C_E.
$$

Therefore successive terms of $4^{-r}h([2^r]P)$ differ by at most $C_E4^{-r-1}$, and the limit is well defined.

Shifting the limit immediately gives $\widehat h([2]P)=4\widehat h(P)$. The addition formula likewise gives

$$
h(P+Q)+h(P-Q)=2h(P)+2h(Q)+O_E(1).
$$

Apply this to $[2^r]P,[2^r]Q$, divide by $2\cdot4^r$, and pass to the limit to obtain the exact [parallelogram law](../../../../../../parallelogram-law.md)

$$
\widehat h(P+Q)+\widehat h(P-Q)=2\widehat h(P)+2\widehat h(Q).
$$

Taking $Q=P$ starts an induction on $|n|$ that yields

$$
\widehat h([n]P)=n^2\widehat h(P)
$$

for every integer $n$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 125](../../../paper-125-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
