# Stable construction of a Givens rotation

↑ **Parent:** [Givens rotation](givens-rotation.md)

For finite [real numbers](real-number.md) $a,b$, a [Givens rotation](givens-rotation.md) that annihilates $b$ is defined mathematically by

$$
r=\operatorname{hypot}(a,b)=\sqrt{a^2+b^2},\qquad
(c,s)=\begin{cases}(a/r,b/r),&r>0,\\(1,0),&a=b=0.\end{cases}
$$

Here `hypot` means an evaluation of the [Euclidean norm](euclidean-norm.md) of $(a,b)^T$ designed to avoid unnecessary range failures in [floating-point arithmetic](floating-point-arithmetic-split.md). The zero case selects the [identity matrix](identity-matrix.md), avoiding division by zero. If $a=0,b\ne0$, then $c=0,s=\operatorname{sign}(b)$; if $b=0,a\ne0$, then $c=\operatorname{sign}(a),s=0$. Thus the retained component is nonnegative, including when $a<0$. In exact arithmetic, $ca+sb=r$ and $-sa+cb=0$.

Computing the [square root](square-root.md) of `a*a + b*b` directly can fail even when the final [norm](norm.md) is representable. In binary64 [floating-point arithmetic](floating-point-arithmetic-split.md), $a=b=10^{308}$ makes the squares overflow, whereas $r\approx1.4142\times10^{308}$ is finite. With $a=b=10^{-300}$ the squares round to zero, although $r\approx1.4142\times10^{-300}$ is representable. A range-safe `hypot` avoids these intermediate failures.

The simple divisions $a/r,b/r$ still need care when $r$ is a [subnormal number](subnormal-number.md): rounding $r$ can cause large relative errors. For the smallest positive binary64 [subnormal number](subnormal-number.md) $\eta=2^{-1074}$, taking $a=b=\eta$ rounds $\sqrt2\eta$ to $\eta$; dividing by that rounded value gives $c=s=1$, which is not an [orthogonal matrix](orthogonal-matrix.md). For nonzero finite inputs, compute the [coefficients](coefficient.md) before rescaling the [norm](norm.md):

$$
t=\max(|a|,|b|),\qquad \alpha=a/t,\quad\beta=b/t,\quad
h=\operatorname{hypot}(\alpha,\beta),\qquad
c=\alpha/h,\quad s=\beta/h,\quad r=th.
$$

At least one scaled component has [absolute value](absolute-value.md) one, and $1\leq h\leq\sqrt2$. This construction keeps the [coefficients](coefficient.md) meaningful even when rounding $r$ is severe. It cannot make an unrepresentably large $r$ finite, preserve an arbitrarily tiny $s$ against underflow, or repair inputs already rounded to zero. The row updates themselves can also overflow if their exact results exceed the available range.

LAPACK's `DLARTG` uses scaling for [numerical stability](stability-of-a-numerical-method.md) but a different sign convention: for $a\ne0$ it chooses $r=\operatorname{sign}(a)\sqrt{a^2+b^2}$ and $c\geq0$; for $b=0$ it returns $c=1,s=0,r=a$. Its block still has the lower-left minus sign. Do not combine its returned [coefficients](coefficient.md) with an assumed nonnegative $r$.[DLARTG, LAPACK 3.12.1, Purpose: block, signed R, scaling and zero-input cases; implementation lines 137–159](dlartg-lapack-3-12-1-by-edward-anderson.md)

## ↑ Ancestors (6)

1. [Givens rotation](givens-rotation.md)
2. [Numerical analysis](numerical-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)
