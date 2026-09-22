# Radial flux through a truncated unit sphere

↑ **Parent:** [Flux integral](flux-integral.md)

Let $-1<s<1$ and let $S_s$ be the outward-oriented boundary of $x^2+y^2+z^2\leq1$, $z\leq s$. For a continuous [function](function-split.md) $h:[-1,s]\to\mathbb R$, the [vector field](vector-field.md) $\mathbf F=h(z)(x,y,z)^T$ has outward [flux](flux.md)

$$
\Phi_h(s)=2\pi\int_{-1}^sh(z)\,dz+\pi s(1-s^2)h(s).
$$

On the curved unit [sphere](sphere.md), the outward [unit normal](unit-normal.md) is $(x,y,z)^T$, so the normal component is $h(z)$. A horizontal spherical band has [area](surface-area.md) $2\pi\,dz$, producing the first term. On the top [disk](disk-mathematics.md), the outward [unit normal](unit-normal.md) is $(0,0,1)^T$, the normal component is $sh(s)$, and the [area](surface-area.md) is $\pi(1-s^2)$, producing the second term.

For $h=f'$ with a continuous first [derivative](derivative.md), the [fundamental theorem of calculus](fundamental-theorem-of-calculus.md) gives

$$
\Phi_{f'}(s)=2\pi\bigl(f(s)-f(-1)\bigr)+\pi s(1-s^2)f'(s).
$$

This direct [surface integral](surface-integral.md) proof needs no second [derivative](derivative.md) of $f$. For $h=1$, it reduces to $\pi(2+3s-s^3)$; the [divergence theorem](divergence-theorem.md) identifies this with three times the enclosed [volume](volume.md).

## ↑ Ancestors (10)

1. [Flux integral](flux-integral.md)
2. [Surface integral](surface-integral.md)
3. [Vector calculus](vector-calculus.md)
4. [Multivariable calculus](multivariable-calculus-split.md)
5. [Calculus](calculus-split.md)
6. [Real analysis](real-analysis-split.md)
7. [Analysis](analysis-split.md)
8. [Area of mathematics](area-of-mathematics.md)
9. [Mathematics](mathematics-split.md)
10. [Codex Wiki](split.md)
