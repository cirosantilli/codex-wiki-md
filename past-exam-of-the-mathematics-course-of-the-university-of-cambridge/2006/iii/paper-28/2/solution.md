<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

For $\sigma>1$, the absolutely convergent logarithm of the [Euler product](../../../../../euler-product.md) for the [Riemann zeta function](../../../../../riemann-zeta-function.md) is

$$
\log\zeta(s)=\sum_p\sum_{k\ge1}\frac{p^{-ks}}k.
$$

The elementary identity $3+4\cos v+\cos2v=2(1+\cos v)^2\ge0$ therefore gives

$$
\log\left(\zeta(\sigma)^3|\zeta(\sigma+it)|^4|\zeta(\sigma+2it)|\right)
=\sum_p\sum_{k\ge1}\frac{3+4\cos(kt\log p)+\cos(2kt\log p)}{kp^{k\sigma}}\ge0.
$$

Thus the expression inside the logarithm is at least one. The [Meromorphic continuation of the Riemann zeta function to the right half-plane](../../../../../meromorphic-continuation-of-the-riemann-zeta-function-to-the-right-half-plane.md) has only a simple [pole](../../../../../pole.md) at one, of [residue](../../../../../residue.md) one. It follows, for example, from

$$
\zeta(s)=\frac{s}{s-1}-s\int_1^\infty\frac{\{u\}}{u^{s+1}}\,du\qquad(\operatorname{Re}s>0),
$$

whose integral is holomorphic there.

Suppose $t\ne0$ and $\zeta$ has a zero of order $m\ge1$ at $1+it$. As $\sigma\downarrow1$, the real factor is $O((\sigma-1)^{-3})$, the middle factor is $O((\sigma-1)^{4m})$, and the factor at $1+2it$ is bounded. Their product would tend to zero, contradicting its lower bound one. Hence

$$
\boxed{\zeta(1+it)\ne0\quad(t\ne0).}
$$

At $t=0$ there is a [pole](../../../../../pole.md), not a zero; the statement about the line does not assert a finite value for $\zeta(1)$. This proves the [three-four-one product proof of zeta boundary nonvanishing](../../../../../three-four-one-product-proof-of-zeta-boundary-nonvanishing.md).

To relate the [Second Chebyshev function](../../../../../second-chebyshev-function.md) to the [logarithmic derivative](../../../../../logarithmic-derivative.md), differentiate the [Euler product](../../../../../euler-product.md) in its half-plane of [absolute convergence](../../../../../absolute-convergence.md):

$$
-\frac{\zeta'(s)}{\zeta(s)}=\sum_{n\ge1}\frac{\Lambda(n)}{n^s}.
$$

Since $\psi(u)=\sum_{n\le u}\Lambda(n)$, its [first integral of the Chebyshev function](../../../../../first-integral-of-the-chebyshev-function.md) is

$$
\Psi_1(x)=\int_0^x\psi(u)\,du=\sum_{n\le x}(x-n)\Lambda(n).
$$

For any fixed $c>1$, its [Mellin inversion formula](../../../../../mellin-inversion-theorem.md) is

$$
\boxed{\Psi_1(x)=\frac1{2\pi i}\int_{c-i\infty}^{c+i\infty}-\frac{\zeta'(s)}{\zeta(s)}\frac{x^{s+1}}{s(s+1)}\,ds.}
$$

For justification, the elementary contour kernel is $\frac1{2\pi i}\int_{(c)}y^s/(s(s+1))\,ds=1-y^{-1}$ for $y>1$ and zero for $0<y\le1$. Close left or right and take the [residues](../../../../../residue.md) at zero and minus one; at $y=1$ the continuous value is zero. [Absolute convergence](../../../../../absolute-convergence.md) on $\operatorname{Re}s=c$ allows termwise integration of the [Dirichlet series](../../../../../dirichlet-series.md), and multiplying this kernel by $x$ gives $(x-n)_+$.

Here is how the relation yields the asymptotic. Move the contour to the left, using the [functional equation of the Riemann zeta function](../../../../../functional-equation-of-the-riemann-zeta-function.md) to control the left-hand side. The [residue](../../../../../residue.md) at $s=1$ is $x^2/2$, and a [Nontrivial zero of the Riemann zeta function](../../../../../nontrivial-zero-of-the-riemann-zeta-function.md) $\rho$ contributes $-x^{\rho+1}/(\rho(\rho+1))$, multiplied by its [multiplicity](../../../../../multiplicity-mathematics.md). The kernel [poles](../../../../../pole.md) at zero and minus one contribute $-x\log(2\pi)$ and $\zeta'(-1)/\zeta(-1)$; a [trivial zero of the Riemann zeta function](../../../../../trivial-zero-of-the-riemann-zeta-function.md) $-2k$ contributes $-x^{1-2k}/(2k(2k-1))$. Thus the [smoothed explicit formula for the Chebyshev function](../../../../../smoothed-explicit-formula-for-the-chebyshev-function.md) is

$$
\Psi_1(x)=\frac{x^2}{2}-\sum_\rho\frac{x^{\rho+1}}{\rho(\rho+1)}-x\log(2\pi)+\frac{\zeta'(-1)}{\zeta(-1)}-\sum_{k\ge1}\frac{x^{1-2k}}{2k(2k-1)}.
$$

For the contour argument, use heights avoiding the zero ordinates and then let those heights increase. The local zero bound from the [Riemann–von Mangoldt formula](../../../../../riemann-von-mangoldt-formula.md), together with the [Local partial-fraction expansion of the Riemann zeta logarithmic derivative](../../../../../local-partial-fraction-expansion-of-the-riemann-zeta-logarithmic-derivative.md), permits heights with logarithmic-derivative bound $O(\log^2 T)$ in each fixed vertical strip. The horizontal integrals then vanish because the denominator is of size $T^2$. After that, send the left edge through negative odd integers to minus infinity; the [functional equation of the Riemann zeta function](../../../../../functional-equation-of-the-riemann-zeta-function.md) bounds the [logarithmic derivative](../../../../../logarithmic-derivative.md) there by a logarithm, and $x^{s+1}$ makes the left integral vanish for fixed $x>1$. This explains why this smoothing allows a convergent contour calculation without a quantitative zero-free region.

In fact the [Riemann–von Mangoldt formula](../../../../../riemann-von-mangoldt-formula.md), stated in the next solution, gives $N(T)=O(T\log T)$ and hence

$$
\sum_\rho\frac1{|\rho(\rho+1)|}<\infty.
$$

The [Nontrivial zeros of the Riemann zeta function](../../../../../nontrivial-zero-of-the-riemann-zeta-function.md) satisfy $0<\operatorname{Re}\rho<1$, using the [Euler product](../../../../../euler-product.md), the [functional equation of the Riemann zeta function](../../../../../functional-equation-of-the-riemann-zeta-function.md), and the nonvanishing just proved. For each such zero, $x^{\rho-1}\to0$ as $x\to\infty$, whereas $|x^{\rho-1}|\le1$ for $x\ge1$. The [dominated convergence theorem](../../../../../dominated-convergence-theorem.md) therefore makes the absolutely convergent zero sum, divided by $x^2$, tend to zero. All the other displayed terms are $o(x^2)$. We obtain

$$
\boxed{\int_0^x\psi(u)\,du\sim\frac{x^2}{2}.}
$$

It remains to unsmooth; differentiating an asymptotic without justification would not suffice. [Monotonicity](../../../../../monotonic-function.md) of $\psi$ gives, for fixed $0<h<1$,

$$
\frac{\Psi_1(x)-\Psi_1((1-h)x)}{hx}\le\psi(x)\le\frac{\Psi_1((1+h)x)-\Psi_1(x)}{hx}.
$$

Divide by $x$ and use the integral asymptotic. The lower and upper limits lie between $1-h/2$ and $1+h/2$. Letting $h\downarrow0$ proves $\psi(x)\sim x$. Higher [prime powers](../../../../../prime-power.md) contribute $O(\sqrt x\log x)$, as in the first solution, so $\vartheta(x)\sim x$. Finally [partial summation](../../../../../abel-s-summation-formula.md) gives

$$
\pi(x)=\frac{\vartheta(x)}{\log x}+\int_2^x\frac{\vartheta(t)}{t(\log t)^2}\,dt.
$$

The integral is $O(x/(\log x)^2)$, by $\vartheta(t)=O(t)$ and splitting at $\sqrt x$. Hence

$$
\boxed{\pi(x)\sim\frac{x}{\log x},}
$$

which is the [Prime number theorem](../../../../../prime-number-theorem.md).

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 28](../../paper-28-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
