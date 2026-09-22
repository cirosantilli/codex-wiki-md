<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The [mean-field approximation](../../../../../mean-field-approximation.md) replaces each site's fluctuating surroundings by a self-consistent average. On a [cubic lattice](../../../../../cubic-lattice.md) each spin has [coordination number of a lattice](../../../../../coordination-number-of-a-lattice.md) $z=2D$, even though summing only over positive basis directions counts each bond once. Write $\sigma_n=M+\delta\sigma_n$ and drop products of deviations. Each Ising bond becomes $\sigma_n\sigma_m\simeq M\sigma_n+M\sigma_m-M^2$, so the approximate [statistical Hamiltonian](../../../../../statistical-hamiltonian.md) is

$$
H_{\rm MF}=-zJM\sum_n\sigma_n+\frac{NzJ}{2}M^2.
$$

The constant corrects counting each bond twice. The resulting independent-spin [partition function](../../../../../canonical-partition-function.md) is $Z_{\rm MF}=e^{-\beta_TNzJM^2/2}[2\cosh(\beta_TzJM)]^N$, where $\beta_T=1/(k_BT)$. The one-spin probabilities give

$$
\langle\sigma\rangle=\frac{e^{\beta_TzJM}-e^{-\beta_TzJM}}{e^{\beta_TzJM}+e^{-\beta_TzJM}}.
$$

Equating this average with the assumed $M$ gives

$$
\boxed{M=\tanh\!\left(\frac{2DJM}{k_BT}\right),\qquad T_c=\frac{2DJ}{k_B}.}
$$

Here $J>0$ is assumed; a ferromagnetic [order parameter](../../../../../order-parameter.md) is not the appropriate choice for an antiferromagnetic coupling. Put $A=T_c/T$. For $A\leq1$, $\tanh(AM)<AM\leq M$ at any $M>0$, so only $M=0$ is possible. For $A>1$, the function $\tanh(AM)-M$ has positive slope at zero, is [strictly concave](../../../../../strictly-concave-function.md) on $M>0$ and is negative at $M=1$. It therefore has exactly one positive zero and a spin-reversed negative zero. Expanding at the bifurcation gives

$$
0=(A-1)M-\frac{A^3M^3}{3}+O(M^5),\qquad M^2=\frac{3(A-1)}{A^3}+O((A-1)^2)\sim3\frac{T_c-T}{T_c}.
$$

The transition is continuous, with [order-parameter critical exponent](../../../../../order-parameter-critical-exponent.md) $\beta=1/2$. Stability can also be checked from the [Bragg-Williams free energy of the Ising model](../../../../../bragg-williams-free-energy-of-the-ising-model.md) per [Ising spin](../../../../../ising-spin-variable.md):

$$
f_{\rm BW}(M)=-\frac{zJ}{2}M^2+k_BT\left\{\frac{1+M}{2}\log\frac{1+M}{2}+\frac{1-M}{2}\log\frac{1-M}{2}\right\}.
$$

Its [derivative](../../../../../derivative.md) is $-zJM+k_BT\operatorname{arctanh}M$, giving the same [self-consistency equation](../../../../../self-consistency-equation.md). Near zero,

$$
f_{\rm BW}(M)=-k_BT\log2+\frac{k_BT-zJ}{2}M^2+\frac{k_BT}{12}M^4+O(M^6).
$$

The quartic coefficient is positive at $T_c$, the stable minima approach zero continuously, and the minimized [free energy](../../../../../thermodynamic-free-energy.md) has no first-derivative jump. Thus **[mean-field approximation](../../../../../mean-field-approximation.md) predicts a second-order transition at $T_c=2DJ/k_B$**. This is the [mean-field Ising critical bifurcation](../../../../../mean-field-ising-critical-bifurcation.md).

For short-range interactions, large dimension gives many neighbours and suppresses the relative fluctuations of their average. More quantitatively, [Gaussian field theory](../../../../../gaussian-field-theory.md) fluctuations averaged over a [correlation volume](../../../../../correlation-volume.md) have [variance](../../../../../variance-split.md) of order $\xi^{2-D}$, while the squared ordinary mean-field [order parameter](../../../../../order-parameter.md) is of order $|t|\sim\xi^{-2}$. Their ratio is proportional to $\xi^{4-D}$. The [Ginzburg criterion](../../../../../ginzburg-criterion.md) therefore makes neglect of critical fluctuations asymptotically consistent above four dimensions, inconsistent below four, and marginal at four, where logarithms occur. Large dimension is a route to validity; sufficiently long-range or infinite-range interactions can also produce mean-field behaviour. In low-dimensional short-range systems even the existence and location of a transition can differ from this approximation.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 51](../../paper-51-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
