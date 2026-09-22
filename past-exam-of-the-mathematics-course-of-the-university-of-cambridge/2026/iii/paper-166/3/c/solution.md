<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $f$ be the monic cubic minimal polynomial of the [algebraic integer](../../../../../../algebraic-integer.md) $\alpha$, let $\alpha_1=\alpha,\alpha_2,\alpha_3$ be its conjugates, and let $\beta_1=\beta,\beta_2$ be the two conjugates of a nonrational $\beta\in\mathcal O_K$. Because the degrees three and two are coprime, the fields are [linearly disjoint](../../../../../../linear-disjointness.md), and

$$
m=N_{\mathbb Q(\alpha)K/\mathbb Q}(\alpha-\beta)
=\prod_{i=1}^3\prod_{j=1}^2(\alpha_i-\beta_j)
$$

is a nonzero [integer](../../../../../../integer.md).

Assume

$$
|\alpha-\beta|\leq H(\beta)^{-(6-\varepsilon)}.
$$

For large $H(\beta)$ this makes $\beta_1$ bounded. Since $\beta$ is a quadratic [algebraic integer](../../../../../../algebraic-integer.md), the [height-Mahler measure formula](../../../../../../height-mahler-measure-formula.md) gives

$$
H(\beta)^2=\max(1,|\beta_1|)\max(1,|\beta_2|),
$$

and therefore $|\beta_2|\asymp H(\beta)^2$. The two remaining factors with $j=1$ are bounded, while the three factors with $j=2$ are $O(|\beta_2|)$. Consequently

$$
1\leq|m|
\leq C_{\alpha,K}|\alpha-\beta|\,|\beta_2|^3
\leq C_{\alpha,K}H(\beta)^\varepsilon.
$$

We now use the standard effective [norm form](../../../../../../norm-form.md) consequence of Part (b). For

$$
L=\mathbb Q(\alpha)K,
\qquad
V=\operatorname{span}_{\mathbb Q}\{1,\alpha,\omega\},
$$

where $1,\omega$ is an integral basis of $K$, the [effective norm-form height estimate](../../../../../../effective-norm-form-height-estimate.md) supplies effective constants $A,C>0$, depending only on $\alpha$ and $K$, such that

$$
H(z)\leq C|N_{L/\mathbb Q}(z)|^A
$$

for every nonzero $z\in V\cap\mathcal O_L$. Its proof factors $(z)$, balances a generator using the [Dirichlet unit theorem](../../../../../../dirichlet-s-unit-theorem.md), and applies the [Baker lower bound for a homogeneous linear form in logarithms](../../../../../../baker-lower-bound-for-a-homogeneous-linear-form-in-logarithms.md) to the linear relations defining $V$; the coprime degrees $3$ and $2$ exclude a unit-family degeneracy.

Apply this estimate to $z=\alpha-\beta$. Since $\beta=\alpha-z$, the height inequalities imply $H(\beta)\leq2H(\alpha)H(z)$. Hence

$$
H(\beta)
\leq C'|m|^A
\leq C''H(\beta)^{A\varepsilon}.
$$

Choose the effective value $\varepsilon=1/(2A)$. The last inequality bounds $H(\beta)$ effectively. The rational integers $\beta\in\mathbb Z$ are already covered by the stronger degree-three [Liouville approximation theorem](../../../../../../liouville-approximation-theorem.md), and the [Northcott theorem](../../../../../../northcott-theorem.md) leaves only finitely many remaining quadratic integers of bounded height. Taking the minimum of

$$
|\alpha-\beta|H(\beta)^{6-\varepsilon}
$$

over this effective finite set gives an effective $c>0$ and proves

$$
|\alpha-\beta|\geq cH(\beta)^{-(6-\varepsilon)}
$$

for every $\beta\in\mathcal O_K$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 166](../../../paper-166-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
