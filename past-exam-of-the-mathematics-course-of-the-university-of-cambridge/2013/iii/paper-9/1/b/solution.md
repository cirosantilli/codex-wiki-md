<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

It is enough to prove the stronger planar [Kakeya maximal function](../../../../../../kakeya-maximal-function.md) bound

$$
\boxed{\|\mathcal K_\delta f\|_{L^2(S^1)}
\lesssim\sqrt{\log(2/\delta)}\,\|f\|_{L^2(\mathbb R^2)}.}
$$

We first work with a $\delta$-separated net of unoriented directions $e_1,\ldots,e_M$, with $M\asymp\delta^{-1}$. Write $\alpha_{ij}$ for angular distance modulo $\pi$. Choose arbitrary length-one, width-$\delta$ rectangles $T_j$ in these directions. The permitted rectangle intersection fact is

$$
|T_i\cap T_j|\lesssim\min\left(\delta,\frac{\delta^2}{\alpha_{ij}}\right)
\lesssim\frac{\delta^2}{\delta+\alpha_{ij}}.
$$

The first alternative includes parallel rectangles. Their locations are arbitrary; only separation of their directions matters.

Define $Af(j)=\delta^{-1}\int_{T_j}f$, and put $\|a\|_{\ell^2_\delta}^2=\delta\sum_j|a_j|^2$. With these weights the [adjoint operator](../../../../../../adjoint-operator.md) is $A^*a=\sum_j a_j\mathbf1_{T_j}$. Since a separated angular net has only a bounded number of directions at each distance scale $k\delta$ from $e_i$, its overlap matrix satisfies

$$
\sum_j|T_i\cap T_j|
\lesssim\delta+\sum_{k=1}^{O(\delta^{-1})}\frac{\delta}{k}
\lesssim\delta\log(2/\delta).
$$

The diagonal term is of size $\delta$. Using $|a_i a_j|\le(|a_i|^2+|a_j|^2)/2$ and symmetry gives the [Schur test](../../../../../../schur-test.md) estimate

$$
\begin{aligned}
\|A^*a\|_2^2
&\le\sum_{i,j}|a_i a_j|\,|T_i\cap T_j|\\
&\lesssim\delta\log(2/\delta)\sum_i|a_i|^2
=\log(2/\delta)\|a\|_{\ell^2_\delta}^2.
\end{aligned}
$$

By [duality of Lp spaces](../../../../../../duality-of-lp-spaces.md), $\|Af\|_{\ell^2_\delta}\lesssim\sqrt{\log(2/\delta)}\|f\|_2$. This is uniform over every choice of the translated rectangles. For each direction choose a rectangle approaching the supremum for $|f|$, then take the limit. That gives the same estimate for the discretized [Kakeya maximal function](../../../../../../kakeya-maximal-function.md).

To recover all directions, partition the direction circle into arcs of length comparable to $\delta$, each with a net direction. A tube in an arc is contained in a rectangle in its net direction with width $C\delta$ and length at most two. A bounded subdivision in the length direction reduces this to the same averaging operators; the wider tubes obey the same overlap estimate with fixed-factor changes. Therefore

$$
\int_{S^1}|\mathcal K_\delta f(e)|^2\,de
\lesssim\delta\sum_j|\mathcal K_{C\delta}^{\mathrm{net}}f(e_j)|^2
\lesssim\log(2/\delta)\|f\|_2^2.
$$

Finally $\sqrt{\log(2/\delta)}\le C_\varepsilon\delta^{-\varepsilon}$ for every $\varepsilon>0$. **The [planar Kakeya maximal estimate](../../../../../../planar-kakeya-maximal-estimate.md) therefore has the required arbitrary small power loss.**

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 9](../../../paper-9-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
