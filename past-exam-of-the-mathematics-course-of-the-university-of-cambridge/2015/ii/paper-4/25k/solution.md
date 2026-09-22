<h1 id="25k/solution">Solution</h1>

↑ **Parent:** [25K](../25k.md)

Treat the [white noise](../../../../../white-noise.md) as innovations with conditional mean zero and conditional second moment $v$, independent of the chosen past control. This is the convention needed for the [dynamic programming](../../../../../dynamic-programming.md) calculation. The printed stage cost is $\tfrac12x^2+u^2$, not one-half of both terms.

With terminal value $V_0(x)=x^2$, induction in the [Bellman equation](../../../../../bellman-equation.md) gives

$$
V_h(x)=\min_u\{\tfrac12x^2+u^2+\mathbb E V_{h-1}(x+u+\epsilon)\}.
$$

If $V_{h-1}(z)=z^2+(h-1)v$, completing the square yields

$$
\tfrac12x^2+u^2+(x+u)^2+hv=x^2+2(u+x/2)^2+hv.
$$

Thus $\boxed{V_h(x)=x^2+hv,\quad u^*(x)=-x/2}$ for every horizon, in particular $V_6(x_0)=x_0^2+6v$. The same completion gives the average-cost [Bellman equation](../../../../../bellman-equation.md) solution $\boxed{\phi(x)=x^2,\quad\lambda=v}$, up to an additive constant in $\phi$.

For every policy in $P$, conditional second moments satisfy $\mathbb E[x_{t+1}^2\mid\mathcal F_t]=(x_t+u_t)^2+v\leq0.9x_t^2+v$. Iterating gives

$$
\mathbb E_\pi x_t^2\leq0.9^t x_0^2+v\sum_{j=0}^{t-1}0.9^j\leq\boxed{x_0^2+10v}.
$$

The Bellman inequality implies $\mathbb E_\pi\sum_{t<h}(\tfrac12x_t^2+u_t^2)\geq hv+x_0^2-\mathbb E_\pi x_h^2$. Dividing by $h$ and using the bound proves that every admissible policy has lower limiting average cost at least $v$, even if its ordinary limit does not exist. The feedback $u=-x/2$ belongs to $P$ because $(x+u)^2=x^2/4\leq0.9x^2$. It makes the Bellman inequality an equality, and its bounded terminal second moment proves its average cost tends to $\boxed{v}$. Therefore it is optimal over $P$.

Merely uncorrelated noise with the displayed unconditional moments would not ensure the conditional identities for arbitrary adapted controls. The innovation interpretation specifies the hypothesis used in the calculation.

## ↑ Ancestors (10)

1. [25K](../25k.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
