<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Work with a nonzero complex unital [Banach algebra](../../../../../banach-algebra-split.md), so $1\ne0$. The [spectrum of an element](../../../../../spectrum-of-an-element.md) is

$$
\sigma_A(x)=\{\lambda\in\mathbb C:\lambda1-x\text{ is not invertible in }A\}.
$$

For $|\lambda|>\|x\|$, the [Neumann series](../../../../../neumann-series.md)

$$
(\lambda1-x)^{-1}=\sum_{n=0}^{\infty}\frac{x^n}{\lambda^{n+1}}
$$

converges in [norm](../../../../../norm.md) and is a two-sided inverse, by multiplying its partial sums and letting the remainder tend to zero. Thus the [spectrum](../../../../../spectrum-functional-analysis.md) lies in $|\lambda|\le\|x\|$. The assumed openness of the invertible group makes its complement closed, so the [spectrum](../../../../../spectrum-functional-analysis.md) is compact.

To prove nonemptiness, suppose every $\lambda$ has an inverse $R(\lambda)=(\lambda1-x)^{-1}$. Locally,

$$
R(\lambda+h)=R(\lambda)(1+hR(\lambda))^{-1}
=\sum_{j\ge0}(-h)^jR(\lambda)^{j+1},
$$

so the resolvent is holomorphic. At infinity its [Neumann series](../../../../../neumann-series.md) gives $\|R(\lambda)\|=O(|\lambda|^{-1})$. For any [bounded linear functional](../../../../../continuous-linear-functional.md) $\ell\in A^*$, the scalar [entire function](../../../../../entire-function.md) $\ell(R(\lambda))$ is bounded: it is bounded on compact disks by continuity, and tends to zero outside them. The [Liouville theorem](../../../../../liouville-theorem.md) makes it constant, and its limit makes that constant zero. The [Hahn-Banach theorem](../../../../../hahn-banach-theorem.md) separates points of the normed space $A$, so $R(\lambda)=0$, contradicting $(\lambda1-x)R(\lambda)=1$. Hence **the [spectrum](../../../../../spectrum-functional-analysis.md) is nonempty and compact**.

On the algebra of [entire functions](../../../../../entire-function.md), set

$$
\boxed{\|f\|_D=\sup_{|z|\le1}|f(z)|.}
$$

It is finite, homogeneous and satisfies the [triangle inequality](../../../../../triangle-inequality.md) and [submultiplicativity](../../../../../submultiplicativity.md). If it vanishes, the [identity theorem](../../../../../identity-theorem.md) makes $f$ identically zero, so it is an [algebra norm](../../../../../algebra-norm.md). However, no [algebra norm](../../../../../algebra-norm.md) on the entire-function algebra can be complete. The coordinate function $Z(z)=z$ satisfies $\sigma(Z)=\mathbb C$ algebraically: $Z-\lambda$ vanishes at $z=\lambda$ and has no entire multiplicative inverse. A complete [algebra norm](../../../../../algebra-norm.md) would make this a [Banach algebra](../../../../../banach-algebra-split.md), contradicting the proved boundedness of its [spectrum](../../../../../spectrum-functional-analysis.md). This is the [entire function algebra admits no complete algebra norm](../../../../../entire-function-algebra-admits-no-complete-algebra-norm.md) obstruction; it applies to every proposed complete [algebra norm](../../../../../algebra-norm.md), not only the displayed one.

For all [continuous functions](../../../../../continuous-function.md) on $\mathbb C$, choose continuous cutoffs

$$
h_n(z)=\begin{cases}
1,&|z-3n|\le1/2,\\
2(1-|z-3n|),&1/2<|z-3n|<1,\\
0,&|z-3n|\ge1.
\end{cases}
$$

Their supports are disjoint and escape every compact set. Thus $f(z)=\sum_{n\ge1}nh_n(z)$ is a locally finite sum and is continuous. Let $g_n(z)=\max(0,1-4|z-3n|)$. This nonzero [continuous function](../../../../../continuous-function.md) is supported where $h_n=1$ and all the other cutoffs vanish. Hence $fg_n=ng_n$. Any [algebra norm](../../../../../algebra-norm.md) would imply

$$
n\|g_n\|=\|fg_n\|\le\|f\|\|g_n\|,
$$

so $n\le\|f\|$ for every positive integer, impossible. Therefore **the algebra of all [continuous functions](../../../../../continuous-function.md) on $\mathbb C$ admits no [algebra norm](../../../../../algebra-norm.md)**, even an incomplete one. This proves the [continuous functions on the complex plane admit no algebra norm](../../../../../continuous-functions-on-the-complex-plane-admit-no-algebra-norm.md) obstruction directly.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 6](../../paper-6-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
