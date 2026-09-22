<h1 id="3/2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For a bounded $C^1$ [classical solution](../../../../../../../classical-solution.md) and a smooth convex entropy $\eta$, let its [entropy flux for a scalar conservation law](../../../../../../../entropy-flux-for-a-scalar-conservation-law.md) satisfy $\psi'=f'\eta'$. The [chain rule](../../../../../../../chain-rule.md) gives

$$
\partial_t\eta(u)+\partial_x\psi(u)=\eta'(u)\bigl(u_t+f'(u)u_x\bigr)=0.
$$

Integration against a nonnegative [test function](../../../../../../../test-function.md), including its initial boundary contribution, gives equality in the entropy inequality. Approximate a convex piecewise $C^1$ entropy by smooth convex functions on the bounded state range. Their values and flux antiderivatives converge uniformly, so the integrated equality passes to the limit. Therefore **every bounded classical solution is an entropy solution**. The bounded qualifier is required by the definition's $L^\infty$ membership; an arbitrary unbounded $C^1$ solution would not satisfy that membership condition.

Conversely, the affine entropies $\eta_+(z)=z$ and $\eta_-(z)=-z$ are both convex, with fluxes $f$ and $-f$. Their inequalities force the same linear weak integral to be both nonnegative and nonpositive. It is therefore zero for every nonnegative test, hence for every test by subtraction of nonnegative compactly supported tests. Thus $\boxed{\text{entropy solution}\Longrightarrow\text{weak solution}.}$ No assumption that the flux itself is convex is used.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [3](../../../3.md)
4. [Paper 105](../../../../paper-105-split.md)
5. [Iii](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
