<h1 id="4/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use the following general [Banach algebra](../../../../../../banach-algebra-split.md) facts: in a complex commutative unital [Banach algebra](../../../../../../banach-algebra-split.md), [maximal ideals](../../../../../../maximal-ideal.md) are exactly the kernels of [algebra characters](../../../../../../character-of-an-algebra.md), meaning nonzero complex multiplicative [linear functionals](../../../../../../linear-functional.md). Such a character satisfies $\phi(1)=1$ and $|\phi(f)|\le\|f\|$, hence is continuous. The [maximal ideal space](../../../../../../maximal-ideal-space-of-a-commutative-banach-algebra.md) is given the [Gelfand topology](../../../../../../gelfand-topology.md), that is, pointwise convergence of characters on algebra elements. These facts follow from closedness of maximal ideals, the [Gelfand-Mazur theorem](../../../../../../gelfand-mazur-theorem.md) for their quotients, and the spectral bound for character values. They do not identify any of the three spaces by themselves.

For the [Wiener algebra](../../../../../../wiener-algebra.md), write $f=\sum_{n\in\mathbb Z}a_nu^n$, where $u(e^{it})=e^{it}$ and $\|f\|_A=\sum|a_n|$. The [Fourier series](../../../../../../fourier-series-split.md) converges absolutely in the algebra norm. If $\phi$ is a character, set $z=\phi(u)$. Since $u$ is invertible and $\|u\|_A=\|u^{-1}\|_A=1$, multiplicativity and the norm bound give $|z|\le1$, $|z^{-1}|\le1$. Thus $|z|=1$. Continuity now gives

$$
\phi(f)=\sum_{n\in\mathbb Z}a_nz^n=f(z).
$$

Conversely, for every $z\in\mathbb T$, evaluation is nonzero, linear and multiplicative, and $|f(z)|\le\sum|a_n|$ makes it continuous. Distinct $z$ give distinct characters because they have different values on $u$. Hence **the character space of the Wiener algebra is the circle**.

For the [analytic Wiener algebra](../../../../../../analytic-wiener-algebra.md), the same expression uses only $n\ge0$. A character is again determined by $z=\phi(u)$, but $u^{-1}$ is no longer in this algebra, so only $|z|\le1$ is forced. Continuity gives $\phi(f)=\sum_{n\ge0}a_nz^n$. Conversely, every $z$ in the closed [unit disk](../../../../../../unit-disk.md) defines evaluation on this absolutely convergent [power series](../../../../../../power-series.md). It is bounded and multiplicative, since multiplication of the series is absolutely convergent [discrete convolution](../../../../../../discrete-convolution.md). Distinct $z$ again differ on $u$. Therefore **the character space of the analytic Wiener algebra is the closed disk**, including its interior and boundary, not just the original boundary circle.

For $C(\mathbb T)$ with the [supremum norm](../../../../../../supremum-norm.md), let $M=\ker\phi$ for a character. Suppose the functions in $M$ had no common zero. At each point choose some $f\in M$ nonzero there. Continuity supplies a neighborhood where it remains nonzero; compactness gives a finite subcover associated to $f_1,\ldots,f_k\in M$. Then

$$
g=\sum_{j=1}^k f_j\overline{f_j}=\sum_{j=1}^k|f_j|^2
$$

is continuous and strictly positive everywhere. It belongs to $M$ because $M$ is an ideal, but it is invertible in $C(\mathbb T)$ with continuous inverse $1/g$. This would imply $1\in M$, a contradiction. There is therefore a common zero $z$ of $M$. The point-evaluation kernel $I_z=\{f:f(z)=0\}$ is maximal, and $M\subseteq I_z$ forces equality. Since $\phi(1)=1$, writing $f=f(z)1+(f-f(z)1)$ then proves $\phi(f)=f(z)$. Conversely every evaluation is a character, and $u$ distinguishes the points. Thus **the character space of continuous functions on the circle is the circle**.

These are topological identifications as well as bijections. The evaluation map $z\mapsto\phi_z$ is continuous for the [Gelfand topology](../../../../../../gelfand-topology.md), because each fixed algebra element is a continuous function of $z$: absolute convergence gives uniform convergence on the circle or closed disk in the first two cases. The parameter spaces are compact, while the character spaces are Hausdorff as subspaces of the pointwise topology. A continuous bijection from a compact space to a Hausdorff space is a [homeomorphism](../../../../../../homeomorphism.md). Consequently the three [maximal ideal spaces](../../../../../../maximal-ideal-space-of-a-commutative-banach-algebra.md) are, respectively,

$$
\boxed{\mathcal M_{A(\mathbb T)}\cong\mathbb T,\qquad\mathcal M_{A^+(\mathbb T)}\cong\overline{\mathbb D},\qquad\mathcal M_{C(\mathbb T)}\cong\mathbb T.}
$$

In each case the maximal ideal associated to a point is the kernel of the evaluation just described. The spelling “Weiner” in the source refers to the [Wiener algebra](../../../../../../wiener-algebra.md).

## ↑ Ancestors (11)

1. [I](../i.md)
2. [4](../../4.md)
3. [Paper 6](../../../paper-6-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
