<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Put $\delta=-A^2-A^{-2}$. The reduced [Kauffman bracket](../../../../../kauffman-bracket.md) is the [Laurent polynomial](../../../../../laurent-polynomial.md) determined by $\langle\bigcirc\rangle=1$, $\langle D\sqcup\bigcirc\rangle=\delta\langle D\rangle$, and the crossing expansion $\langle D\rangle=A\langle D_A\rangle+A^{-1}\langle D_B\rangle$. Fix the A smoothing so that a positive curl has multiplier $-A^3$; rotating the local crossing interchanges the smoothing descriptions. Equivalently, its [bracket smoothing states](../../../../../bracket-smoothing-state.md) give

$$
\boxed{\langle D\rangle=\sum_sA^{a(s)-b(s)}\delta^{|s|-1},}
$$

where $a(s)$ and $b(s)$ count its A and B smoothings and $|s|$ is the number of state [circles](../../../../../circle.md). Resolving all crossings proves that the recursive rules define the same [polynomial](../../../../../polynomial-split.md) independently of the order of expansion.

Under a positive [Reidemeister move](../../../../../reidemeister-move.md) of type I, the two resolutions give $A\delta+A^{-1}=-A^3$ times the straight strand; the negative curl gives $A^{-1}\delta+A=-A^{-3}$. Thus the bracket itself is not an unframed [link invariant](../../../../../link-invariant.md). For type II, use the adjacent cap-cup generator $e$ of the [Temperley-Lieb algebra](../../../../../temperley-lieb-diagram-algebra.md), with $e^2=\delta e$. The crossing and its inverse are $R=A1+A^{-1}e$ and $R^{-1}=A^{-1}1+Ae$, and

$$
RR^{-1}=1+(A^2+A^{-2}+\delta)e=1.
$$

For type III, $e_ie_{i+1}e_i=e_i$ and the analogous reversed relation give

$$
R_iR_{i+1}R_i-R_{i+1}R_iR_{i+1}=A^{-1}(A^2+\delta+A^{-2})(e_i-e_{i+1})=0.
$$

Hence the bracket is invariant under types II and III.

For an oriented diagram, let $w(D)$ be its [writhe of a link diagram](../../../../../writhe-of-a-link-diagram.md), the sum of its signed crossings. Types II and III preserve [writhe of a link diagram](../../../../../writhe-of-a-link-diagram.md), while a positive or negative curl changes it by one or minus one. The [Jones polynomial](../../../../../jones-polynomial.md) is therefore

$$
\boxed{V_L(t)=(-A^3)^{-w(D)}\langle D\rangle,\qquad t=A^{-4},\qquad V_{\bigcirc}=1.}
$$

The normalization cancels type I, so all [Reidemeister moves](../../../../../reidemeister-move.md) preserve it. It is a [Laurent polynomial](../../../../../laurent-polynomial.md) in $t^{1/2}$; its breadth means the largest occurring t exponent minus the smallest, including half-integral exponents for [links](../../../../../link.md).

The [Jones polynomial skein relation](../../../../../jones-polynomial-skein-relation.md) follows directly from the same normalization. Write $S$ for the bracket of the [oriented smoothing](../../../../../oriented-smoothing.md) and $H$ for the other smoothing. The local expansions are $\langle D_+\rangle=AS+A^{-1}H$ and $\langle D_-\rangle=A^{-1}S+AH$, while $w(D_\pm)=w(D_0)\pm1$. Consequently

$$
A^4V_{L_+}-A^{-4}V_{L_-}=(-A^3)^{-w(D_0)}(A^{-2}-A^2)S.
$$

Substituting $t=A^{-4}$ gives

$$
\boxed{t^{-1}V_{L_+}-tV_{L_-}+(t^{-1/2}-t^{1/2})V_{L_0}=0.}
$$

The other smoothing has cancelled, so the identity applies with exactly the oriented local convention in the PDF.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 19](../../paper-19-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
