<h1 id="3/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

For $t>0$, write $\Phi$ for the [standard normal distribution function](../../../../../../standard-normal-distribution-function.md). Since the [Brownian running maximum](../../../../../../brownian-running-maximum.md) is nonnegative, $a\leq0$ gives simply $\mathbb P(B_t\leq b)=\Phi(b/\sqrt t)$.

For $a>0$ and $b<a$, reflect the [Brownian motion](../../../../../../brownian-motion-split.md) after its first hit of $a$. This is a [stopping time](../../../../../../stopping-time.md), and the [Strong Markov property](../../../../../../strong-markov-property.md) together with symmetry of Brownian increments shows that reflection preserves its law. On paths that hit $a$, it sends the endpoint $B_t$ to $2a-B_t$. Thus the event with endpoint at most $b$ maps to endpoints at least $2a-b$, all of which necessarily hit $a$. This proves

$$
\mathbb P(M_t\geq a,B_t\leq b)=\mathbb P(B_t\geq2a-b)=\Phi((b-2a)/\sqrt t).
$$

The same reflection gives $\mathbb P(M_t\geq a)=2(1-\Phi(a/\sqrt t))$. If $b\geq a$, every path with $B_t>b$ has hit $a$, so subtracting that endpoint tail gives the complete answer:

$$
\boxed{\mathbb P(M_t\geq a,B_t\leq b)=
\begin{cases}
\Phi(b/\sqrt t),&a\leq0,\\
\Phi((b-2a)/\sqrt t),&a>0,\ b<a,\\
1-2\Phi(a/\sqrt t)+\Phi(b/\sqrt t),&a>0,\ b\geq a.
\end{cases}}
$$

The expressions agree at $b=a$. This is the [joint distribution of Brownian motion and its running maximum](../../../../../../joint-distribution-of-brownian-motion-and-its-running-maximum.md). In particular $M_t$ has the distribution of $|B_t|$ and has no atoms for $t>0$. If $t=0$, the pair is $(0,0)$ deterministically, so the requested probability is $\mathbf1_{\{a\leq0,\ b\geq0\}}$.

## ↑ Ancestors (11)

1. [2](../2.md)
2. [3](../../3.md)
3. [Paper 26](../../../paper-26-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
