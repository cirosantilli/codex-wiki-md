<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $X=I+E$. Use a submultiplicative [Sobolev algebra](../../../../../../sobolev-algebra.md) [norm](../../../../../../norm.md) for which the Fourier projections are contractive, and its compatible [matrix](../../../../../../matrix.md)/column [norms](../../../../../../norm.md). The numeric hypothesis $\|E\|<1$ is understood in this algebra [norm](../../../../../../norm.md); the unscaled Fourier [Sobolev norm](../../../../../../sobolev-norm.md) need not have multiplication constant one.

Let $A_{>0}$ and $A_{<0}$ denote the strictly positive and strictly negative Fourier subspaces. The equation $y_+=-P_{>0}(E+Ey_+)$ is a contraction on $M_n(A_{>0})$, so it has a unique solution. Put $Y_+=I+y_+$ and $Z_-=XY_+$. The equation says $Z_-\in M_n(A_-)$, and $Y_+(0)=I$. Similarly the contraction $v_-=-P_{<0}(E+v_-E)$ gives $V_-=I+v_-$ with $Z_+=V_-X\in M_n(A_+)$. No invertibility of these solutions has yet been assumed.

Now $V_-Z_-=Z_+Y_+$ belongs to both Fourier subalgebras, hence is a constant [matrix](../../../../../../matrix.md) $C$. Taking constant coefficients on either side shows $C=Z_-(0)=Z_+(0)$. We claim $C$ is invertible. If $Cv=0$, then the Hardy compression $T_X=P_{\geq0}X$ annihilates $Y_+v$, because $P_{\geq0}Z_-v=Cv=0$. But $T_X=I+P_{\geq0}E$ on the Hardy [Sobolev space](../../../../../../sobolev-space-split.md) has inverse given by a [Neumann series](../../../../../../neumann-series.md), since the perturbation has [norm](../../../../../../norm.md) less than one. Thus $Y_+v=0$, and its constant coefficient is $v$, forcing $v=0$. Finite-dimensionality proves the claim.

Consequently $C^{-1}Z_+$ is a left inverse of $Y_+$, and $C^{-1}V_-$ is a left inverse of $Z_-$. [Matrix](../../../../../../matrix.md) entries are functions in a commutative algebra, so pointwise finite-dimensional inversion makes these left inverses two-sided inverses in their respective Fourier subalgebras. Set

$$
\boxed{X_-=Z_-,\qquad X_+=Y_+^{-1}.}
$$

Then $X=X_-X_+$, both factors are invertible in the stated algebras, and $X_+(0)=I$. If two normalized factorizations exist, $\widetilde X_-^{-1}X_-=\widetilde X_+X_+^{-1}$ lies in $A_-\cap A_+$ and is constant; evaluating the analytic side at zero makes it $I$. This proves uniqueness. The argument is [near-identity Sobolev loop factorization](../../../../../../near-identity-sobolev-loop-factorization.md) and, crucially, proves invertibility rather than treating the contraction solution itself as automatically invertible.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 10](../../../paper-10-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
