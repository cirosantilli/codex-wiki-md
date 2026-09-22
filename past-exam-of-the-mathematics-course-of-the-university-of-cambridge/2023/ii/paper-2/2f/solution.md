<h1 id="2f/solution">Solution</h1>

↑ **Parent:** [2F](../2f.md)

For a continuous closed path $\gamma:[0,1]\to\mathbb C\setminus\{0\}$, choose a continuous argument lift

$$
\frac{\gamma(t)}{|\gamma(t)|}=e^{2\pi i\theta(t)}.
$$

Its [winding number of a continuous closed path](../../../../../winding-number-of-a-continuous-closed-path.md) about zero is

$$
w(\gamma,0)=\theta(1)-\theta(0)\in\mathbb Z.
$$

For a piecewise smooth path this equals $(2\pi i)^{-1}\int_\gamma dz/z$.

If $|\gamma(t)|>|\phi(t)|$, then

$$
H(s,t)=\gamma(t)+s\phi(t),\qquad 0\leq s\leq1,
$$

never vanishes, since $|H(s,t)|\geq|\gamma(t)|-s|\phi(t)|>0$. Thus $H$ is a homotopy through closed paths avoiding zero. By [homotopy invariance of winding number](../../../../../homotopy-invariance-of-winding-number.md), or directly by the [dominated-perturbation lemma](../../../../../dominated-perturbation-preserves-winding-number.md),

$$
w(\gamma+\phi,0)=w(\gamma,0).
$$

More generally, $\gamma_0$ and $\gamma_1$ are homotopic by paths in $\Gamma$ when there is a [continuous function](../../../../../continuous-function.md)

$$
H:[0,1]^2\longrightarrow\mathbb C\setminus\{0\}
$$

with $H(0,t)=\gamma_0(t)$, $H(1,t)=\gamma_1(t)$, and $H(s,0)=H(s,1)$ for every $s$. The winding-number theorem states that such a homotopy implies

$$
w(\gamma_0,0)=w(\gamma_1,0).
$$

For the [Fundamental theorem of algebra](../../../../../fundamental-theorem-of-algebra.md), let $P(z)=a_nz^n+\cdots+a_0$ with $n\geq1$. For sufficiently large $R$,

$$
|a_nR^ne^{2\pi int}|>
|a_{n-1}R^{n-1}e^{2\pi i(n-1)t}+\cdots+a_0|
$$

for every $t$. The dominated-perturbation lemma shows that $t\mapsto P(Re^{2\pi it})$ has the same winding number as $t\mapsto a_nR^ne^{2\pi int}$, namely $n$. If $P$ had no zero, however,

$$
H(s,t)=P(sRe^{2\pi it})
$$

would be a homotopy in $\Gamma$ from that loop to the constant loop $P(0)$, whose winding number is zero. This contradiction proves that $P$ has a complex root. This is the [winding-number proof of the fundamental theorem of algebra](../../../../../winding-number-proof-of-the-fundamental-theorem-of-algebra.md).

Finally suppose that a continuous retraction $r:D^2\to S^1$ existed. The boundary loop $\eta(t)=e^{2\pi it}$ has winding number one, while $(1-s)\eta(t)$ contracts it to zero inside the [disc](../../../../../topological-disc.md). Composing this contraction with $r$ gives a homotopy through loops in $S^1$ from $r\circ\eta=\eta$ to the constant loop $r(0)$. Their winding numbers are respectively one and zero, contradicting homotopy invariance. Hence there is no such retraction, as in the [winding-number proof of the no-retraction theorem](../../../../../winding-number-proof-of-the-no-retraction-theorem.md).

## ↑ Ancestors (10)

1. [2F](../2f.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
