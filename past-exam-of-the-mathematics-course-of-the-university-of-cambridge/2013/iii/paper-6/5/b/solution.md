<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The shear $(t,x,v)\mapsto(t,x+tv,v)$ is a smooth [diffeomorphism](../../../../../../diffeomorphism.md) with [determinant](../../../../../../determinant.md) one and sends compact sets to compact sets. Thus $F,G$ are [locally integrable functions](../../../../../../locally-integrable-function.md). On a compact time interval $I$ and compact label set $K\subset\mathbb R^6$, the [integral](../../../../../../integral.md) $\int_K\int_I|G|\,dt\,dx\,dv$ is finite. The [Fubini theorem](../../../../../../fubini-s-theorem.md), followed by a countable exhaustion of time intervals and label sets, shows that $G(\cdot,x,v)\in L^1_{\rm loc}(\mathbb R)$ for almost every $(x,v)$.

To transform the weak equation, choose $\phi(t,x,v)=\rho(x-tv,v)\psi(t)$, where $\rho\in C_c^\infty(\mathbb R^6)$ and $\psi\in C_c^\infty(\mathbb R)$. Including a velocity cutoff in $\rho$ ensures the required [compact support](../../../../../../compact-support.md). The transport [derivative](../../../../../../derivative.md) of this [test function](../../../../../../test-function.md) is $\rho(x-tv,v)\psi'(t)$. Change variables to the characteristic labels to obtain

$$
\int\rho(x,v)\left[\int\bigl(F(t,x,v)\psi'(t)+G(t,x,v)\psi(t)\bigr)\,dt\right]dx\,dv=0.
$$

The fundamental test-function identity makes the bracket zero almost everywhere. Choose a countable dense family of time [test functions](../../../../../../test-function.md) on each bounded interval and extend by continuity; there is then a single negligible label set outside which $\partial_tF=G$ as one-dimensional distributions.

For each remaining label, subtract the primitive $H(t)=\int_0^tG(s)\,ds$. The [distributional derivative](../../../../../../distributional-derivative.md) of $F-H$ is zero, so it is a constant almost everywhere. Choose the resulting [absolutely continuous representative along free characteristics](../../../../../../absolutely-continuous-representative-along-free-characteristics.md), $\widetilde F(t)=C+H(t)$. The [fundamental theorem of calculus](../../../../../../fundamental-theorem-of-calculus.md) gives

$$
\boxed{\widetilde F(t_2,x,v)-\widetilde F(t_1,x,v)=\int_{t_1}^{t_2}G(s,x,v)\,ds\quad\text{for all }t_1,t_2}.
$$

The representative qualification is essential: an arbitrary locally integrable representative can be modified on one time slice without changing the distributional equation, and would not satisfy the identity for every pair of times.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 6](../../../paper-6-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
