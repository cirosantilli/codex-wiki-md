<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

First continue the [Riemann zeta function](../../../../../riemann-zeta-function.md) into $\Re s>0$. Summing the integral of the integer-part function gives, initially for $\Re s>1$,

$$
\zeta(s)=s\int_1^\infty\lfloor u\rfloor u^{-s-1}\,du
=\frac{s}{s-1}-s\int_1^\infty\{u\}u^{-s-1}\,du.
$$

The last integral defines a [holomorphic function](../../../../../holomorphic-function.md) for $\Re s>0$, so this continuation has only a simple [pole](../../../../../pole.md) at one, of [residue](../../../../../residue.md) one.

For $\sigma>1$, logarithmic expansion of the [Euler product](../../../../../euler-product.md) and $3+4\cos v+\cos2v=2(1+\cos v)^2\ge0$ give

$$
3\log\zeta(\sigma)+4\log|\zeta(\sigma+it)|+\log|\zeta(\sigma+2it)|
=\sum_p\sum_{j\ge1}\frac{3+4\cos(jt\log p)+\cos(2jt\log p)}{jp^{j\sigma}}\ge0.
$$

This proves the [three-four-one product proof of zeta boundary nonvanishing](../../../../../three-four-one-product-proof-of-zeta-boundary-nonvanishing.md) inequality

$$
\zeta(\sigma)^3|\zeta(\sigma+it)|^4|\zeta(\sigma+2it)|\ge1.
$$

If $t\ne0$ and $\zeta(1+it)=0$ to order $r\ge1$, the middle factor is $O((\sigma-1)^{4r})$, the first is $O((\sigma-1)^{-3})$, and the last remains bounded. Their product tends to zero, a contradiction. At $t=0$ there is a [pole](../../../../../pole.md), not a zero. **The zeta function has no zero on $\Re s=1$.**

Put $I(x)=\int_0^x\psi(u)\,du=\sum_{n\le x}(x-n)\Lambda(n)$, where $\Lambda$ is the [Von Mangoldt function](../../../../../von-mangoldt-function.md). Logarithmic differentiation of the [Euler product](../../../../../euler-product.md) gives $-\zeta'(s)/\zeta(s)=\sum_n\Lambda(n)n^{-s}$ for $\Re s>1$. The [first integral of the Chebyshev function](../../../../../first-integral-of-the-chebyshev-function.md) is consequently

$$
\boxed{I(x)=\frac1{2\pi i}\int_{c-i\infty}^{c+i\infty}
-\frac{\zeta'(s)}{\zeta(s)}\frac{x^{s+1}}{s(s+1)}\,ds,\qquad c>1.}
$$

To check its kernel, evaluate the [contour integral](../../../../../contour-integral.md) of $y^s/(s(s+1))$ by closing to the left for $y>1$ and to the right for $0<y<1$. The [residues](../../../../../residue.md) at zero and minus one give $1-y^{-1}$ in the first case and zero in the second. Multiplication by $x$ and substitution $y=x/n$ therefore produce $(x-n)_+$. On the line $c>1$, the [Dirichlet series](../../../../../dirichlet-series.md) and vertical integral have [absolute convergence](../../../../../absolute-convergence.md), justifying their interchange; at $x=n$ the kernel is zero on either side.

Here is the smoothing step that establishes the requested asymptotic. Shift the line of this [contour integral](../../../../../contour-integral.md) to the left. The [pole](../../../../../pole.md) of $-\zeta'/\zeta$ at one has [residue](../../../../../residue.md) $+1$; at each [Nontrivial zero of the Riemann zeta function](../../../../../nontrivial-zero-of-the-riemann-zeta-function.md) $\rho$ of [zero multiplicity](../../../../../multiplicity-of-a-zero.md) $m_\rho$ its [residue](../../../../../residue.md) is $-m_\rho$. The denominators also contribute at zero and minus one, and the [trivial zeros of the Riemann zeta function](../../../../../trivial-zero-of-the-riemann-zeta-function.md) occur at $-2,-4,\ldots$. Summing these [residues](../../../../../residue.md) yields the [smoothed explicit formula for the Chebyshev function](../../../../../smoothed-explicit-formula-for-the-chebyshev-function.md)

$$
I(x)=\frac{x^2}2-\sum_\rho\frac{x^{\rho+1}}{\rho(\rho+1)}
-x\log(2\pi)+\frac{\zeta'(-1)}{\zeta(-1)}
-\sum_{k\ge1}\frac{x^{1-2k}}{2k(2k-1)}.
$$

Zeros are repeated with [zero multiplicity](../../../../../multiplicity-of-a-zero.md). For the limits of the [contour integral](../../../../../contour-integral.md), choose horizontal heights avoiding zero ordinates, where the logarithmic derivative on each fixed strip is $O((\log T)^2)$. The factor $s(s+1)$ makes their integrals tend to zero. On left edges chosen a fixed distance from the trivial zeros, the [functional equation of the Riemann zeta function](../../../../../functional-equation-of-the-riemann-zeta-function.md) controls the logarithmic derivative by $O(\log(|s|+2))$; for fixed $x>1$ the remaining vertical integral vanishes as that edge moves left. This is why the extra integration of $\psi$ is useful.

The [Riemann–von Mangoldt formula](../../../../../riemann-von-mangoldt-formula.md), stated in Question 3, gives $N(T)=O(T\log T)$, hence

$$
\sum_\rho\frac1{|\rho(\rho+1)|}<\infty.
$$

Indeed each dyadic height block contributes $O((\log T)/T)$. The zero-free line just proved, the nonvanishing [Euler product](../../../../../euler-product.md) on its right, and the [functional equation of the Riemann zeta function](../../../../../functional-equation-of-the-riemann-zeta-function.md) put every [Nontrivial zero of the Riemann zeta function](../../../../../nontrivial-zero-of-the-riemann-zeta-function.md) in $0<\Re\rho<1$. Therefore each $x^{\rho-1}$ tends to zero, with absolute value at most one for $x\ge1$. Divide the explicit formula by $x^2$ and use [dominated convergence](../../../../../dominated-convergence-theorem.md) on the zero terms with [absolute convergence](../../../../../absolute-convergence.md). The remaining displayed terms are $o(x^2)$, and we obtain

$$
\boxed{I(x)\sim x^2/2.}
$$

Monotonicity of $\psi$ removes the smoothing. For $0<h<1$,

$$
\frac{I(x)-I((1-h)x)}{hx}\le\psi(x)
\le\frac{I((1+h)x)-I(x)}{hx}.
$$

After division by $x$, the limits of the two bounds are $1-h/2$ and $1+h/2$. Let $h\downarrow0$ to get $\psi(x)\sim x$. Question 1 gives $\psi(x)-\vartheta(x)=O(\sqrt x\log x)=o(x)$, so $\vartheta(x)\sim x$. [Partial summation](../../../../../abel-s-summation-formula.md) now gives

$$
\pi(x)=\frac{\vartheta(x)}{\log x}+\int_2^x\frac{\vartheta(t)}{t(\log t)^2}\,dt
\sim\frac{x}{\log x}.
$$

The integral is $O(x/(\log x)^2)$, by splitting at $\sqrt x$ and using $\vartheta(t)=O(t)$. Inverting this at $x=p_n$, we have $n\sim p_n/\log p_n$ and hence $\log n\sim\log p_n$. Thus **the $n$th [prime](../../../../../prime-number.md) satisfies**

$$
\boxed{p_n\sim n\log n.}
$$

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 22](../../paper-22-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
