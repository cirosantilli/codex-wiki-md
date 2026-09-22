<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For a null momentum, use [light cone gauge](../../../../../../light-cone-gauge.md) to remove potential components along one null direction; the free field equations remove the remaining longitudinal components. The physical polarizations of a [massless p-form gauge field](../../../../../../massless-p-form-gauge-field.md) are therefore antisymmetric tensors on the $D-2$ transverse directions, transforming under the rotational [little group](../../../../../../little-group.md) $SO(D-2)$. Choosing $p$ distinct transverse indices gives

$$
\boxed{n_p(D)=\binom{D-2}{p}.}
$$

This already takes account of the reducibility of the higher-form gauge parameter; naïvely subtracting just one gauge-parameter component count would not give the right answer. No self-duality constraint is being imposed.

For [dimensional reduction](../../../../../../dimensional-reduction.md) to four dimensions, retain the zero modes on a flat $(D-4)$-torus, without fluxes or projections. Write $d=D-4$ and split tensor indices into spacetime indices $\mu$ and internal indices $i$. A component with $r$ spacetime indices is a four-dimensional $r$-form, with $p-r$ internal indices and hence multiplicity $\binom d{p-r}$. The complete field decomposition is

$$
A_p\longrightarrow\bigoplus_{r=0}^{\min(p,4)}\binom d{p-r}\ A_r^{(4)}.
$$

Use the convention that a binomial coefficient vanishes when its lower entry lies outside its range. In four dimensions the scalar, vector and two-form have respectively $1,2,1$ local polarizations, while the three- and four-form potentials have none. Hence [toroidal reduction of a p-form gauge field](../../../../../../toroidal-reduction-of-a-p-form-gauge-field.md) gives

$$
\begin{aligned}
n_{\rm reduced}&=\binom dp+2\binom d{p-1}+\binom d{p-2}\\
&=\sum_r\binom2r\binom d{p-r}=\binom{d+2}p=\binom{D-2}p.
\end{aligned}
$$

The middle identity follows by comparing the coefficient of $t^p$ in $(1+t)^2(1+t)^d=(1+t)^{d+2}$. Therefore

$$
\boxed{n_{\rm reduced}=n_p(D).}
$$

A four-dimensional two-form may instead be counted as one scalar by [two-form scalar duality](../../../../../../two-form-scalar-duality.md), with the same result. Higher-form zero modes can describe nondynamical flux data, which are distinct from these propagating degrees of freedom. Nonzero [Kaluza-Klein modes](../../../../../../kaluza-klein-mode.md) form massive lower-dimensional multiplets with longitudinal components supplied by the associated gauge fields; the displayed matching concerns the massless zero-mode sector.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 53](../../../paper-53-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
