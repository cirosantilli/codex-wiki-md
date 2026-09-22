<h1 id="3/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

The [option delta](../../../../../../option-delta.md) is a derivative in $S$, not in $x$. With $d=e^{-r(T-t)}$, the logarithmic chain rule gives

$$
\Delta=d e^{-x}u_x,\qquad \Gamma=d e^{-2x}(u_{xx}-u_x).
$$

Thus use $\Delta_i=d e^{-x_i}D_xu_i$ for the [delta hedge](../../../../../../delta-hedge.md), and $\Gamma_i=d e^{-2x_i}(D_{xx}u_i-D_xu_i)$ for [option gamma](../../../../../../option-gamma.md). These formulas also identify the [finite-difference option Greeks](../../../../../../finite-difference-option-greeks.md) correctly on the equally spaced log-price grid.

There are two distinct accuracy statements. A smooth exact function has central first- and second-derivative truncation errors of order $h^2$. But the computed values themselves have error $e_i=O(h^2)$ under the coupled refinement. Without further control on its spatial variation,

$$
|D_xe_i|\leq\frac{|e_{i+1}|+|e_{i-1}|}{2h}=O(h),\qquad
|D_{xx}e_i|\leq\frac{|e_{i+1}|+2|e_i|+|e_{i-1}|}{h^2}=O(1).
$$

Therefore **the value error bound alone guarantees only first-order delta accuracy and does not guarantee convergent gamma**. For example grid error $e_i=h^2\sin(\pi i/2)$ has a central first difference of order $h$ and a second difference of order one, despite second-order value accuracy.

If instead the scheme has a smooth error expansion $e_i=h^2E(x_i,t)+o(h^2)$ with corresponding derivative bounds, both Greeks can retain second-order accuracy at smooth interior points. Hence reliable gamma is possible with additional regularity and a verified Greek refinement, but cannot be inferred merely from the value convergence in part (e). This qualification is important because the stated bounded-volatility assumption supplies no such error-derivative control.

## ↑ Ancestors (11)

1. [F](../f.md)
2. [3](../../3.md)
3. [Paper 48](../../../paper-48-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
