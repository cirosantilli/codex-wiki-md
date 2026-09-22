<h1 id="10d/solution">Solution</h1>

↑ **Parent:** [10D](../10d.md)

The [intermediate value theorem](../../../../../intermediate-value-theorem.md) states that if $f:[a,b]\to\mathbb R$ is [continuous](../../../../../continuous-function.md) and $y$ lies between $f(a)$ and $f(b)$, then some $c\in[a,b]$ satisfies $f(c)=y$.

Assume $f(a)<y<f(b)$ and let

$$
S=\{x\in[a,b]:f(x)\leq y\},
\qquad c=\sup S.
$$

The [least-upper-bound property](../../../../../least-upper-bound-property.md) makes $c$ well defined. If $f(c)<y$, continuity gives points immediately to the right of $c$ in $S$, contradicting that $c$ is an upper bound. If $f(c)>y$, continuity gives a left neighborhood of $c$ disjoint from $S$, contradicting the definition of the [supremum](../../../../../supremum.md). Thus $f(c)=y$. The endpoint and reversed-order cases follow directly or by replacing $f$ with $-f$.

The [mean value theorem](../../../../../mean-value-theorem.md) states that if $g$ is continuous on $[\alpha,\beta]$ and differentiable on $(\alpha,\beta)$, then some $c\in(\alpha,\beta)$ satisfies

$$
g'(c)=\frac{g(\beta)-g(\alpha)}{\beta-\alpha}.
$$

For the functions in the question, the definition of the [derivative](../../../../../derivative.md) makes $h$ continuous at $a$ and $f$ continuous at $b$, with

$$
h(a)=g'(a)<k,
\qquad
h(b)=\frac{g(b)-g(a)}{b-a}=f(a),
\qquad
f(b)=g'(b)>k.
$$

If the middle secant slope equals $k$, take $[\alpha,\beta]=[a,b]$. If it exceeds $k$, the [intermediate value theorem](../../../../../intermediate-value-theorem.md) applied to $h$ gives $\beta\in(a,b)$ with $h(\beta)=k$, and we take $\alpha=a$. If it is below $k$, apply the theorem to $f$ to obtain $\alpha\in(a,b)$ with $f(\alpha)=k$, and take $\beta=b$. In every case

$$
\frac{g(\beta)-g(\alpha)}{\beta-\alpha}=k.
$$

The [mean value theorem](../../../../../mean-value-theorem.md) on this subinterval then produces $c\in(\alpha,\beta)\subset(a,b)$ with

$$
\boxed{g'(c)=k}.
$$

This is the [Darboux theorem for derivatives](../../../../../darboux-s-theorem-analysis.md) for the stated pair of derivative values.

## ↑ Ancestors (10)

1. [10D](../10d.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ia](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
