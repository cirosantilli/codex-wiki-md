<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Itô formula](../../../../../../ito-s-lemma.md) decomposes the smooth transform into a [continuous local martingale](../../../../../../continuous-local-martingale.md) and a [finite-variation process](../../../../../../finite-variation-process.md):

$$
f(M_t)-f(0)=N_t+\frac12\int_0^tf''(M_s)\,d[M]_s,
\qquad N_t=\int_0^tf'(M_s)\,dM_s.
$$

If $f(M)$ has [finite variation](../../../../../../total-variation-of-a-function.md), then $N$ also has [finite variation](../../../../../../total-variation-of-a-function.md). A [continuous finite-variation local martingale is constant](../../../../../../continuous-finite-variation-local-martingale-is-constant.md), so $N=0$ and

$$
0=[N]_t=\int_0^tf'(M_s)^2\,d[M]_s.
$$

It remains to show that the second-order term vanishes; the preceding observation alone does not establish this.

Let $Z=\{a:f'(a)=0\}$. By the [occupation-times formula](../../../../../../occupation-times-formula.md) for the [local time of a semimartingale](../../../../../../local-time-of-a-semimartingale.md),

$$
0=\int_{\mathbb R}f'(a)^2L_t^a(M)\,da.
$$

Therefore $L_t^a(M)=0$ for almost every $a\notin Z$. Also $f''(a)=0$ for almost every $a\in Z$: if $f'(a)=0$ and $f''(a)\ne0$, continuity of $f''$ makes $f'$ strictly monotone in a neighborhood of $a$, so that zero is isolated. Such isolated zeros form a countable [set](../../../../../../set-split.md). Localizing to bounded paths and finite [quadratic variation](../../../../../../quadratic-variation.md), then using the [occupation-times formula](../../../../../../occupation-times-formula.md) once more, gives

$$
\int_0^t|f''(M_s)|\,d[M]_s
=\int_{\mathbb R}|f''(a)|L_t^a(M)\,da=0.
$$

Both terms in the [Itô formula](../../../../../../ito-s-lemma.md) now vanish. Apply this on all rational times and use continuity to obtain the simultaneous conclusion

$$
\boxed{f(M_t)=f(0)\quad\text{for every }t\geq0\text{ almost surely}.}
$$

This is the [finite-variation smooth transform of a continuous local martingale](../../../../../../finite-variation-smooth-transform-of-a-continuous-local-martingale.md) property.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 24](../../../paper-24-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
