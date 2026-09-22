<h1 id="8/solution">Solution</h1>

↑ **Parent:** [8](../8.md)

There are two common normalizations. I will define both explicitly, because the numerical conclusion in the question uses the unreduced one.

Set $\delta=-A^2-A^{-2}$. The reduced [Kauffman bracket](../../../../../kauffman-bracket.md) of a nonempty [link diagram](../../../../../link-diagram.md) is

$$
\langle D\rangle_{\mathrm{red}}
=\sum_s A^{a(s)-b(s)}\delta^{|s|-1},
$$

where $s$ runs over all bracket smoothings, $a(s),b(s)$ count $A$- and $B$-smoothings, and $|s|$ is the number of resulting circles. Locally,

$$
\langle\text{crossing}\rangle
=A\langle A\text{-smoothing}\rangle+A^{-1}\langle B\text{-smoothing}\rangle.
$$

Fix the usual [Kauffman bracket](../../../../../kauffman-bracket.md) convention in which the $A$-smoothing at a positive braid crossing is its [oriented smoothing](../../../../../oriented-smoothing.md); reflecting a crossing exchanges $A$ and $A^{-1}$. The [unknot](../../../../../unknot.md) has reduced bracket $1$, and adjoining another circle multiplies the bracket by $\delta$. The unreduced [Kauffman bracket](../../../../../kauffman-bracket.md) uses $\delta^{|s|}$ instead and assigns the empty diagram $1$. Thus for a nonempty diagram

$$
\langle D\rangle_{\mathrm{un}}=\delta\langle D\rangle_{\mathrm{red}}.
$$

For completeness, the bracket calculations for all three [Reidemeister moves](../../../../../reidemeister-move.md) can be carried out in the [Temperley-Lieb diagram algebra](../../../../../temperley-lieb-diagram-algebra.md). Let $I$ be the identity two-strand [tangle](../../../../../tangle.md), and let $e$ be the cap-cup [tangle](../../../../../tangle.md). Composition gives $e^2=\delta e$. The two crossings correspond to

$$
R=A I+A^{-1}e,\qquad R^{-1}=A^{-1}I+A e.
$$

Consequently

$$
RR^{-1}=I+(A^2+A^{-2}+\delta)e=I,
$$

which proves invariance under the second [Reidemeister move](../../../../../reidemeister-move.md). On three strands, the cap-cup diagrams satisfy $e_1e_2e_1=e_1$, $e_2e_1e_2=e_2$, and $e_i^2=\delta e_i$. Expand the two sides of the third move. Their difference is

$$
R_1R_2R_1-R_2R_1R_2
=(A+A^{-1}\delta+A^{-3})(e_1-e_2)=0.
$$

Thus the third [Reidemeister move](../../../../../reidemeister-move.md) also preserves either bracket normalization. Reflected forms of these moves follow by replacing $A$ with $A^{-1}$.

A positive curl contributes $A\delta+A^{-1}=-A^3$, and a negative curl contributes $A^{-1}\delta+A=-A^{-3}$. The [writhe of a link diagram](../../../../../writhe-of-a-link-diagram.md) $w(D)$ changes by $+1$ or $-1$ in exactly these cases. Therefore the corrected bracket

$$
f_D(A)=(-A^3)^{-w(D)}\langle D\rangle
$$

is invariant under the first [Reidemeister move](../../../../../reidemeister-move.md) as well; the second and third moves leave the [writhe of a link diagram](../../../../../writhe-of-a-link-diagram.md) unchanged. Substituting $t=A^{-4}$ defines a [Jones polynomial](../../../../../jones-polynomial.md). For multiple components half-integer powers of $t$ may occur. The reduced version $V_L^{\mathrm{red}}$ has $V_U^{\mathrm{red}}=1$, and the [Unreduced Jones polynomial](../../../../../unreduced-jones-polynomial.md) is

$$
V_L^{\mathrm{un}}(t)=-(t^{1/2}+t^{-1/2})V_L^{\mathrm{red}}(t).
$$

At $A=1$, switching a crossing does not change the bracket: both smoothing coefficients are $1$. It changes the [writhe of a link diagram](../../../../../writhe-of-a-link-diagram.md) by $2$, so the correction factor $(-1)^{-w}$ is unchanged. Hence either [Jones polynomial](../../../../../jones-polynomial.md) at $t=1$ is unchanged by a [crossing change](../../../../../crossing-change.md). By switching crossings, any $l$-component [link](../../../../../link.md) can be made an [unlink](../../../../../unlink.md). Its crossing-free diagram has $l$ circles and zero [writhe of a link diagram](../../../../../writhe-of-a-link-diagram.md), giving

$$
\boxed{V_L^{\mathrm{red}}(1)=(-2)^{l-1},\qquad V_L^{\mathrm{un}}(1)=(-2)^l.}
$$

Thus **the printed conclusion $|V_L(1)|=2^l$ holds for the unreduced normalization**. For the reduced [Jones polynomial](../../../../../jones-polynomial.md), the correct conclusion is $\boxed{|V_L^{\mathrm{red}}(1)|=2^{l-1}}$; the [unknot](../../../../../unknot.md) alone already rules out $2^l$ in that convention.

## ↑ Ancestors (10)

1. [8](../8.md)
2. [Paper 16](../../paper-16-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
