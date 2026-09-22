<h1 id="5/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The cross-model target must include a model-order prior $\rho_k$. Write its joint, unnormalized density as

$$
t_k(a,v)=\rho_k\,p(y\mid a,v,k)\,p(a\mid k)\,p(v\mid k).
$$

Here the prior densities are normalized within each model. In particular their $k$-dependent determinants and powers of $2\pi$ cannot be dropped merely because the fixed-model posterior in part (i) was given up to proportionality.

For explicit [birth and death moves for Bayesian variable selection](../../../../../../../birth-and-death-moves-for-bayesian-variable-selection.md), choose a birth with probability $b_k$, generate $u$ from a density $g_k(u\mid a,v)$, append $u$ as the new covariate coefficient, and leave $v$ unchanged. The map from $(a,v,u)$ to $(a',v')=((a,u),v)$ is invertible under the reverse deletion and has absolute Jacobian one. It matches dimensions: the smaller-model coefficients and [variance](../../../../../../../variance-split.md) have dimension $k+2$, and the one auxiliary draw supplies the larger-model dimension $k+3$. If the reverse death is selected with probability $d_{k+1}$, accept with

$$
\boxed{\alpha_b=\min\left\{1,
\frac{t_{k+1}((a,u),v)d_{k+1}}
{t_k(a,v)b_k g_k(u\mid a,v)}\right\}.}
$$

For a death, delete the last coefficient $u$, retain the others and the [variance](../../../../../../../variance-split.md), and use

$$
\boxed{\alpha_d=\min\left\{1,
\frac{t_k(a,v)b_k g_k(u\mid a,v)}
{t_{k+1}((a,u),v)d_{k+1}}\right\}.}
$$

To verify [detailed balance](../../../../../../../detailed-balance.md), multiply the birth acceptance by $t_kb_kg_k$ and the reverse death acceptance by $t_{k+1}d_{k+1}$. Both equal the minimum of these two quantities in the matched coordinates. This proves reversibility without merely naming a dimension-changing algorithm. A more general bijection introduces its absolute Jacobian, and random choices among several covariates introduce the corresponding forward and reverse selection probabilities. Add within-model updates so that coefficients and [variance](../../../../../../../variance-split.md) can explore each model. These are [reversible-jump Markov chain Monte Carlo](../../../../../../../reversible-jump-markov-chain-monte-carlo.md) updates; the unspecified model prior and proposal density must be supplied to implement them numerically.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [5](../../../5.md)
4. [Paper 47](../../../../paper-47-split.md)
5. [Iii](../../../../split.md)
6. [2006](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
