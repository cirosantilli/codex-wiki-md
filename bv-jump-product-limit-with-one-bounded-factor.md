# BV jump-product limit with one bounded factor

↑ **Parent:** [BV slicing theorem](bv-slicing-theorem.md)

Let $a\in BV(\Omega)$, $b\in BV(\Omega)\cap L^\infty(\Omega)$ and $\delta_tc=c\circ\Phi_t-c$, where $\Phi_t$ is the [local flow](local-flow.md) of $\varphi e_j$ with nonnegative $\varphi\in C_c^\infty(\Omega)$. The formula uses common oriented [BV traces on a hypersurface](bv-trace-on-a-hypersurface.md); the trace difference of $a$ is zero almost everywhere on $J_b\setminus J_a$. It also holds for both negative-time increments with denominator positive $t$.

The [BV slicing theorem](bv-slicing-theorem.md) reduces the calculation to one dimension. With a right-continuous representative of $a$ and $\mu=Da$, [Fubini's theorem](fubini-s-theorem.md) yields

$$
\frac1t\int\delta_ta\,\delta_tb=\int\left(\frac1t\int_{\Phi_{-t}(s)}^s\delta_tb(x)\,dx\right)d\mu(s).
$$

The inner factor tends to $\varphi(s)[b](s)$ and is bounded in absolute value by $2\|b\|_\infty\|\varphi\|_\infty$. [Dominated convergence](dominated-convergence-theorem.md) against $|\mu|$ leaves only its [measure atoms](atom-measure-theory.md) at the countable slice jumps of $b$. That same bound times $|Da_y|$ permits integration over the transverse coordinates. No essential bound on $a$ is used, even if its slice values grow without bound. The formula is useful for [opposite-flow fidelity identity for quadratic data](opposite-flow-fidelity-identity-for-quadratic-data.md) with unbounded data and a bounded comparison function.

## ↑ Ancestors (10)

1. [BV slicing theorem](bv-slicing-theorem.md)
2. [Function of bounded variation on a domain](function-of-bounded-variation-on-a-domain.md)
3. [Total variation seminorm on a domain](total-variation-seminorm-on-a-domain.md)
4. [Variational regularization](variational-regularization.md)
5. [Regularization of an inverse problem](regularization-of-an-inverse-problem.md)
6. [Inverse problem](inverse-problem-split.md)
7. [Analysis](analysis-split.md)
8. [Area of mathematics](area-of-mathematics.md)
9. [Mathematics](mathematics-split.md)
10. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Jump-amplitude inequality for a bounded ROF minimizer](jump-amplitude-inequality-for-a-bounded-rof-minimizer.md)
- [No-new-jumps property of total variation denoising](no-new-jumps-property-of-total-variation-denoising.md)
- [Opposite-flow fidelity identity for quadratic data](opposite-flow-fidelity-identity-for-quadratic-data.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-64/2/iii/solution.md)
