<h1 id="4/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $H_0^1$ be the [Cameron-Martin space of Wiener measure](../../../../../../cameron-martin-space-of-wiener-measure.md) on $[0,T]$: its elements start at zero, are absolutely continuous, and have square-integrable derivatives. For $h\in H_0^1$, let $y^h$ solve the controlled [ordinary differential equation](../../../../../../ordinary-differential-equation.md)

$$
\dot y_t^h=\sum_{i=1}^d V_i(y_t^h)\dot h_t^i,\qquad y_0^h=y_0.
$$

The [Stroock-Varadhan support theorem](../../../../../../stroock-varadhan-support-theorem.md) in the uniform topology is

$$
\boxed{\operatorname{supp}\mathcal L(Y)=\overline{\{y^h:h\in H_0^1\}}^{\|\cdot\|_\infty}\subset C_{y_0}([0,T],\mathbb R^e).}
$$

One may equivalently take piecewise linear or smooth controls starting at zero. The skeleton uses the displayed vector fields, as appropriate for the Stratonovich equation.

Choose $2<p<3$ and work in the complete separable space of anchored [geometric p-rough paths](../../../../../../geometric-p-rough-path.md), with its [rough path metric](../../../../../../rough-path-metric.md) $d_p$. The [enhanced Brownian motion](../../../../../../enhanced-brownian-motion.md) is a random element of this space. Its [support of a measure](../../../../../../support-of-a-measure.md) is

$$
K=\overline{\{S_2(h):h\in H_0^1\}}^{d_p}.
$$

We explain this Brownian support step using the permitted results about the enhancement. The almost-sure polygonal convergence proved in Question 3 gives the inclusion of its support in $K$. Indeed, polygonal controls belong to $H_0^1$, and the enhancement belongs to their closed signature closure almost surely. Hölder rough-path convergence at an exponent greater than $1/p$ implies $p$-variation convergence: for the level-$k$ differences, sum the bound proportional to $|t-s|^{kp\alpha/k}=|t-s|^{p\alpha}$ over a partition. Since $p\alpha>1$, these sums are uniformly bounded and tend to zero with the Hölder distance.

For the reverse inclusion, use [Brownian rough path small-ball positivity](../../../../../../brownian-rough-path-small-ball-positivity.md), namely $\mathbb P(d_p(\mathbf B,e)<r)>0$ for every $r>0$, and [Cameron-Martin quasi-invariance of enhanced Brownian motion](../../../../../../cameron-martin-quasi-invariance-of-enhanced-brownian-motion.md). These are the Brownian input results used without proof here. For $h\in H_0^1$, the [rough path translation](../../../../../../rough-path-translation.md) $T_h$ is continuous and sends $e$ to $S_2(h)$. The law of $T_h\mathbf B$ is equivalent to that of $\mathbf B$. Given an open neighborhood $U$ of $S_2(h)$, continuity supplies an identity neighborhood mapped into $U$. Small-ball positivity gives positive probability that $T_h\mathbf B\in U$; equivalence of the two laws gives $\mathbb P(\mathbf B\in U)>0$. Hence $S_2(h)$ belongs to the Brownian support for every $h$. Closedness of support proves the equality with $K$.

Let $\Phi$ be the state-path solution map of the [rough differential equation](../../../../../../rough-differential-equation.md) driven by these vector fields, with the fixed initial value $y_0$. The assumed identification of the Stratonovich solution says $Y=\Phi(\mathbf B)$. Boundedness of the fields and all their derivatives ensures global existence and the regularity needed by the [universal limit theorem](../../../../../../universal-limit-theorem.md). That theorem makes $\Phi$ continuous from the rough-path space into the uniform state-path space. For a control signature, consistency with ordinary equations gives $\Phi(S_2(h))=y^h$.

We use the elementary [support under a continuous map](../../../../../../support-under-a-continuous-map.md) identity

$$
\operatorname{supp}(f_*\mu)=\overline{f(\operatorname{supp}\mu)}.
$$

To prove it, a neighborhood of $f(x)$ with $x\in\operatorname{supp}\mu$ has an open inverse image containing $x$, and therefore positive measure. This puts $f(\operatorname{supp}\mu)$, and its closure, in the image support. Conversely, the image closure is closed and has full image measure, since the original support has full measure. The minimal closed full-measure characterization from Question 4(i) gives the other inclusion.

Apply this identity to $f=\Phi$ and the Brownian rough-path law. We obtain

$$
\operatorname{supp}\mathcal L(Y)=\overline{\Phi(K)}.
$$

Continuity and the definition of $K$ imply $\Phi(K)\subset\overline{\{\Phi(S_2(h)):h\in H_0^1\}}$. The reverse inclusion after taking closures follows from $S_2(h)\in K$. Therefore the last displayed support is exactly the uniform closure of the skeleton paths, proving the theorem.

Finally, piecewise constant and smooth approximations of $\dot h$ converge in $L^2$, hence in $L^1$ on a finite interval. Their controls converge in total variation, their signatures converge in the rough-path metric, and the [universal limit theorem](../../../../../../universal-limit-theorem.md) gives uniform convergence of the corresponding skeleton solutions. This proves the stated equivalence of the control classes.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [4](../../4.md)
3. [Paper 31](../../../paper-31-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
