<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

For a nonzero complex unital [Banach algebra](../../../../../banach-algebra-split.md), define

$$
\sigma_A(x)=\{\lambda\in\mathbb C:\lambda1-x\text{ is not invertible in }A\}.
$$

This is the [spectrum of an element](../../../../../spectrum-of-an-element.md); its complement carries the [resolvent of an element](../../../../../resolvent-of-an-element.md) $R_x(\lambda)=(\lambda1-x)^{-1}$.

If $|\lambda|>\|x\|$, the [Neumann series](../../../../../neumann-series.md)

$$
R_x(\lambda)=\lambda^{-1}\sum_{j=0}^{\infty}(x/\lambda)^j
$$

converges in $A$. Multiplication of finite partial sums followed by a [norm](../../../../../norm.md) limit gives both inverse identities. Thus the spectrum is bounded by $\|x\|$. The invertible set is open by the allowed assumption, and $\lambda\mapsto\lambda1-x$ is continuous, so the spectrum is closed. It is therefore compact if nonempty.

To prove nonemptiness, suppose the resolvent exists for every $\lambda$. At a fixed $\lambda_0$, the same series applied locally gives

$$
R_x(\lambda_0+h)=\sum_{j=0}^{\infty}(-h)^jR_x(\lambda_0)^{j+1}
$$

for $|h|\|R_x(\lambda_0)\|<1$, proving [norm](../../../../../norm.md) analyticity. Every bounded complex [linear functional](../../../../../linear-functional.md) $\psi\in A^*$ therefore gives an entire scalar function $\psi(R_x(\lambda))$. On compact disks it is bounded by continuity of inversion, and the large-$\lambda$ series gives

$$
\|R_x(\lambda)\|\leq\frac{\|1\|}{|\lambda|-\|x\|}\longrightarrow0.
$$

Here the factor $\|1\|\geq1$ handles an [algebra norm](../../../../../algebra-norm.md) whose identity was not normalized to one. The [Liouville theorem](../../../../../liouville-theorem.md) forces each scalar function to be identically zero. The [Hahn-Banach theorem](../../../../../hahn-banach-theorem.md) separates points of $A$, so $R_x(\lambda)=0$, contradicting $(\lambda1-x)R_x(\lambda)=1$. Hence

$$
\boxed{\sigma_A(x)\text{ is nonempty and compact},\qquad \sigma_A(x)\subseteq\{|\lambda|\leq\|x\|\}}.
$$

This includes an explicit proof of the [nonemptiness of the Banach-algebra spectrum](../../../../../nonemptiness-of-the-banach-algebra-spectrum.md) rather than using it as a named result.

For the algebra of [entire functions](../../../../../entire-function.md), choose the [compact-disk algebra norm on entire functions](../../../../../compact-disk-algebra-norm-on-entire-functions.md)

$$
\|f\|=\sup_{|z|\leq1}|f(z)|.
$$

It is finite by continuity on a compact disk, satisfies the [norm](../../../../../norm.md) axioms, and is submultiplicative. If the [norm](../../../../../norm.md) is zero, $f$ vanishes on the open disk, so the [identity theorem](../../../../../identity-theorem.md) gives $f=0$ on the plane. Thus it is an actual [algebra norm](../../../../../algebra-norm.md), not merely a [seminorm](../../../../../seminorm.md).

No complete [algebra norm](../../../../../algebra-norm.md) is possible. For the coordinate function $Z(z)=z$, the function $Z-\lambda1$ has a zero at $\lambda$ for every complex $\lambda$ and hence cannot have a multiplicative inverse among [entire functions](../../../../../entire-function.md). Thus its algebraic spectrum is all of $\mathbb C$, independently of any chosen [norm](../../../../../norm.md). Were an [algebra norm](../../../../../algebra-norm.md) complete, the spectral theorem just proved would make that spectrum bounded, a contradiction. Therefore **[entire functions](../../../../../entire-function.md) admit an [algebra norm](../../../../../algebra-norm.md) but no complete [algebra norm](../../../../../algebra-norm.md)**. This distinguishes failure of every complete [algebra norm](../../../../../algebra-norm.md) from failure of just the displayed disk [norm](../../../../../norm.md).

For continuous functions on the plane, construct disjoint plateaux explicitly. Let

$$
\chi_n(z)=\min\{1,\max\{0,2-8|z-n|\}\},\qquad g_n(z)=\max\{0,1-8|z-n|\},\qquad f(z)=\sum_{n\geq1}n\chi_n(z).
$$

The supports of $\chi_n$ lie in the disks $|z-n|\leq1/4$, so they are pairwise disjoint and form a locally finite family. Thus $f$ is continuous. On the support where $g_n$ is nonzero, $\chi_n=1$ and all other bumps vanish, giving $fg_n=ng_n$; also $g_n(n)=1$, so no $g_n$ is zero. If an [algebra norm](../../../../../algebra-norm.md) existed, [submultiplicativity](../../../../../submultiplicativity.md) would imply

$$
n\|g_n\|=\|fg_n\|\leq\|f\|\|g_n\|,
$$

so $n\leq\|f\|$ for every positive integer, impossible. Consequently **the algebra of all continuous functions on the plane admits no [algebra norm](../../../../../algebra-norm.md)**, with no [completeness](../../../../../completeness.md) hypothesis needed.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 6](../../paper-6-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
