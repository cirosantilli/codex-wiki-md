<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the same [Brownian motion](../../../../../../brownian-motion-split.md) for both solutions: this is a [synchronous coupling](../../../../../../synchronous-coupling.md). For $D_t=X_t-Y_t$, the [Itô formula](../../../../../../ito-s-lemma.md) gives

$$
dD_t^2=\left[2D_t(b(X_t)-b(Y_t))+(\sigma(X_t)-\sigma(Y_t))^2\right]\,dt+2D_t(\sigma(X_t)-\sigma(Y_t))\,dW_t.
$$

On any fixed finite horizon the [stochastic integral](../../../../../../stochastic-integral.md) has mean zero. Indeed, boundedness of $\sigma$ and the assumed second-moment bounds make the expectation of its squared integrand integrable in time. With $h(t)=\mathbb ED_t^2$, the contraction condition yields, for every $s\leq t$,

$$
h(t)\leq h(s)-k\int_s^th(r)\,dr.
$$

The allowed [Gronwall inequality](../../../../../../gronwall-inequality.md) gives the [mean-square contraction of synchronously coupled diffusions](../../../../../../mean-square-contraction-of-synchronously-coupled-diffusions.md)

$$
\boxed{\mathbb E(X_t-Y_t)^2\leq e^{-kt}\mathbb E(X_0-Y_0)^2.}
$$

The identical estimate can also be obtained by localizing the nonnegative local supermartingale $e^{kt}D_t^2$ and using Fatou's lemma, a formulation useful when the drift has linear growth.

There is a genuine compatibility issue in the printed global assumptions. If $|b|\leq B$, then for $d=|x-y|$,

$$
2(x-y)(b(x)-b(y))+(\sigma(x)-\sigma(y))^2\geq-4Bd.
$$

It cannot be at most $-kd^2$ for all $d>4B/k$. Thus **a globally bounded drift cannot satisfy the stated strict contraction on all of the real line**. The stochastic estimate above is the requested conditional calculation. For a non-vacuous application, global boundedness of the drift must be relaxed while retaining suitable existence and moment hypotheses; it is not silently changed here.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [6](../../6.md)
3. [Paper 27](../../../paper-27-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
