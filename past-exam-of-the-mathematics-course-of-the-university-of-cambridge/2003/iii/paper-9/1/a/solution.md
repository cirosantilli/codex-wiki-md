<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Put $\alpha=-\log|c|>0$. Since $f$ has no zeros and the [unit disc](../../../../../../unit-disc.md) is [simply connected](../../../../../../simply-connected-space.md), it has a [holomorphic logarithm](../../../../../../holomorphic-logarithm.md). Thus $F=-\log f$ is [holomorphic](../../../../../../complex-differentiability-at-a-point.md) with $\operatorname{Re}F>0$ and $\operatorname{Re}F(0)=\alpha$. The [Cayley transform between the half-plane and disk](../../../../../../cayley-transform-between-the-half-plane-and-disk.md) gives

$$
\phi(z)=\frac{F(z)-F(0)}{F(z)+\overline{F(0)}}\in\mathbb D,\qquad \phi(0)=0.
$$

The [Schwarz lemma](../../../../../../schwarz-lemma.md) yields $|\phi'(0)|\le1$, so the [Carathéodory derivative bound for the right half-plane](../../../../../../caratheodory-derivative-bound-for-the-right-half-plane.md) gives $|F'(0)|\le2\alpha$. Since $f'=-F'f$, the sharp answer is

$$
\boxed{\max |f'(0)|=2|c|\log\frac1{|c|}.}
$$

Equality in the [Schwarz lemma](../../../../../../schwarz-lemma.md) holds exactly when $\phi(z)=\omega z$, $|\omega|=1$. Solving for $F$ and exponentiating gives exactly the extremizers

$$
\boxed{f(z)=c\exp\left(-\frac{2\alpha\omega z}{1-\omega z}\right),\qquad |\omega|=1.}
$$

Their logarithmic real part is $\alpha\operatorname{Re}[(1+\omega z)/(1-\omega z)]>0$, so each is indeed a zero-free map into the [unit disc](../../../../../../unit-disc.md) with the prescribed value at zero.

For a fixed $w\in\mathbb D$, put $r=|w|$. Apply the [Harnack inequality on the unit disk](../../../../../../harnack-inequality-on-the-unit-disk.md) to the positive [harmonic function](../../../../../../harmonic-function.md) $\operatorname{Re}F$ and then exponentiate its negative. The [zero-free Schwarz lemma](../../../../../../zero-free-schwarz-lemma.md) gives

$$
\boxed{|c|^{(1+r)/(1-r)}\le |f(w)|\le |c|^{(1-r)/(1+r)}.}
$$

For $w\ne0$ both endpoints are attained: take $\omega w=r$ for the lower endpoint and $\omega w=-r$ for the upper endpoint in the displayed extremizers. At zero both are $|c|$. If the question is interpreted as allowing $w$ to vary as well, the sharp [infimum](../../../../../../infimum.md) and [supremum](../../../../../../supremum.md) over all admissible pairs $(f,w)$ are respectively $0$ and $1$, approached as $r\uparrow1$; neither value is attained inside the [unit disc](../../../../../../unit-disc.md). An individual function need not have these global extremal values: the constant function $f=c$ is a simple example.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 9](../../../paper-9-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
