<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the [Itô formula](../../../../../../ito-s-lemma.md) up to $T_n$:

$$
X_{t\wedge T_n}^2
=2\int_0^{t\wedge T_n}X_s\sigma(X_s)\,dB_s
+\int_0^{t\wedge T_n}\bigl(2X_sb(X_s)+\sigma^2(X_s)\bigr)ds.
$$

For fixed $n$, the stopped stochastic integrand is bounded on each finite horizon, so its integral has [expectation](../../../../../../expected-value.md) zero. The [linear growth condition for an SDE](../../../../../../linear-growth-condition-for-an-sde.md) and $2xb(x)\le x^2+b(x)^2$ give

$$
2xb(x)+\sigma^2(x)\le K+(K+1)x^2.
$$

Writing $u_n(t)=\mathbb EX_{t\wedge T_n}^2$, and bounding the active-time integrand by the stopped square, yields

$$
u_n(t)\le Kt+(K+1)\int_0^tu_n(s)\,ds.
$$

The [Gronwall inequality](../../../../../../gronwall-inequality.md) gives a bound independent of $n$:

$$
u_n(t)\le\frac{K}{K+1}\bigl(e^{(K+1)t}-1\bigr)=C_t.
$$

On $\{T_n\le t\}$, continuity gives $|X_{t\wedge T_n}|=n$. The [Markov inequality](../../../../../../markov-inequality.md) therefore gives

$$
\boxed{\mathbb P(T_n\le t)\le C_t/n^2\longrightarrow0}.
$$

Since $T_n\uparrow\xi$, the event $\{\xi\le t\}$ is the intersection of these decreasing events and has probability zero. Taking integer $t$ proves $\xi=\infty$ almost surely. This proves global existence with locally, rather than globally, Lipschitz coefficients under the stated growth bound.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 38](../../../paper-38-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
