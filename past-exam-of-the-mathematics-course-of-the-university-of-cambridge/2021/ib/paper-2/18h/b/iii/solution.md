<h1 id="18h/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Let $h_i=\mathbb E_iT_0$ be the [expected hitting time](../../../../../../../expected-hitting-time.md) of state $0$. For $i\geq1$, [first-step analysis](../../../../../../../first-step-analysis.md) gives

$$
q^{-(i+2)}(h_{i+1}-h_i)
+q^{-i}(h_{i-1}-h_i)=-1.
$$

With $d_i=h_i-h_{i-1}$ this becomes

$$
d_{i+1}-q^2d_i=-q^{i+2}.
$$

The minimal nonnegative solution has

$$
d_i=\frac{q^{i+1}}{q-1},
$$

so

$$
\boxed{\mathbb E_1T_0=h_1=d_1=\frac{q^2}{q-1}}.
$$

Equivalently, [Kac's lemma](../../../../../../../kac-s-lemma.md) gives $\mathbb E_0T_0^+=1/\pi_0$. A first step from $0$ either returns immediately with probability $1-p$ or moves to $1$ with probability $p$, so

$$
\frac1{\pi_0}=1+p\,\mathbb E_1T_0.
$$

Substituting $\pi_0=(q-1)/(q-1+q^2p)$ gives the same result.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [18H](../../../18h.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [Ib](../../../../split.md)
6. [2021](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
