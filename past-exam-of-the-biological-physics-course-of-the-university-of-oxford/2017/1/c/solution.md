<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For the [parameter sensitivity of autorepressed expression](../../../../parameter-sensitivity-of-autorepressed-expression.md), unregulated [production](../../../../gene-expression.md) has $Y_{\rm st}=\beta/\alpha$, so its logarithmic [sensitivity](../../../../sensitivity-analysis.md) is one. In the strong Hill approximation, $Y_{\rm st}=(\beta K^n/\alpha)^{1/(n+1)}$, with $K,\alpha,n$ held fixed. Hence

$$
\boxed{S(Y_{\rm st},\beta)=1\quad\text{without feedback},\qquad
S(Y_{\rm st},\beta)=\frac1{n+1}\quad\text{with strong Hill repression}.}
$$

The ideal logic level $Y_{\rm st}\simeq K$ instead gives $S\simeq0$, because changing [production](../../../../gene-expression.md) primarily changes the switching duty fraction, not the threshold. Finite Hill repression has a residual [production](../../../../gene-expression.md) [sensitivity](../../../../sensitivity-analysis.md).

The exact Hill [steady-state](../../../../steady-state.md) relation makes the comparison continuous. Write $s=(Y_{\rm st}/K)^n$; then $\beta=\alpha Y_{\rm st}(1+s)$ and $d\beta/dY_{\rm st}=\alpha[1+(n+1)s]$. Thus

$$
\boxed{S(Y_{\rm st},\beta)=\frac{1+s}{1+(n+1)s}.}
$$

It tends to one for weak repression and to $1/(n+1)$ for strong repression. The calculation concerns a local relative parameter change, not the response to an arbitrary large [production](../../../../gene-expression.md) perturbation.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the biological physics course of the University of Oxford](../../../split.md)
5. [Biological physics course of the University of Oxford](../../../../biological-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
