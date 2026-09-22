<h1 id="4/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Consider the complex-linear two-coordinate map $H(x,y)=(x+y,x-y)$. The [triangle inequality](../../../../../../triangle-inequality.md) shows that its [operator norm](../../../../../../operator-norm.md) from $\ell^1$ to $\ell^\infty$ is one; equality is attained at $(1,0)$. The complex parallelogram identity

$$
|x+y|^2+|x-y|^2=2(|x|^2+|y|^2)
$$

shows that its [norm](../../../../../../norm.md) from $\ell^2$ to $\ell^2$ is $\sqrt2$. Interpolate these endpoint bounds by the [Riesz-Thorin theorem](../../../../../../riesz-thorin-theorem.md) with parameter $\eta=2/p$. Then

$$
\frac1{p'}=1-\frac{\eta}{2},\qquad
\frac1p=\frac{\eta}{2},\qquad
\|H:\ell^{p'}\to\ell^p\|\leq(\sqrt2)^\eta=2^{1/p}.
$$

Dividing the output [norm](../../../../../../norm.md) by $2^{1/p}$ proves the scalar estimate:

$$
\boxed{\left(\frac{|x+y|^p+|x-y|^p}{2}\right)^{1/p}
\leq(|x|^{p'}+|y|^{p'})^{1/p'}.}
$$

Apply it pointwise to $f,g$ and integrate its $p$th power. With $r=p/p'=p-1>1$, this gives

$$
\left(\frac{\|f+g\|_p^p+\|f-g\|_p^p}{2}\right)^{1/p}
\leq\bigl\||f|^{p'}+|g|^{p'}\bigr\|_r^{1/p'}.
$$

By [Minkowski inequality](../../../../../../minkowski-inequality.md), the expression on the right is at most

$$
\left(\bigl\||f|^{p'}\bigr\|_r+
\bigl\||g|^{p'}\bigr\|_r\right)^{1/p'}
=\left(\|f\|_p^{p'}+\|g\|_p^{p'}\right)^{1/p'}.
$$

Therefore **the requested function inequality holds**, namely the [dual-exponent Clarkson inequality](../../../../../../dual-exponent-clarkson-inequality.md).

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [4](../../4.md)
3. [Paper 5](../../../paper-5-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
