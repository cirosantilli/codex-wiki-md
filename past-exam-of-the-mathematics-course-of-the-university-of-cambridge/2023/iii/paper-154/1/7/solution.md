<h1 id="1/7/solution">Solution</h1>

↑ **Parent:** [7](../7.md)

The scaling in part 5 gives

$$
\|u(t)\|_4^4=\lambda(t)^{-2}\|v\|_4^4
=\frac{\|v\|_4^4}{1+4t^2}.
$$

Thus $u\in L^4_{t,x}([-1,\infty)\times\mathbb R^2)$. For $T<T'$, the dual [Strichartz estimate for the free Schrödinger equation](../../../../../../strichartz-estimate-for-the-free-schrodinger-equation.md) gives

$$
\left\|\int_T^{T'}S(-s)(u|u|^2)(s)\,ds\right\|_2
\lesssim\||u|^2u\|_{L^{4/3}_{t,x}([T,T'])}
=\|u\|_{L^4_{t,x}([T,T'])}^3,
$$

which tends to zero as $T,T'\to\infty$. The integrals in the question are therefore Cauchy in $L^2$.

The [Duhamel principle](../../../../../../duhamel-s-principle.md) in the interaction representation defines an $L^2$ limit $u_\infty$ and expresses $S(-t)u(t)-u_\infty$ as the tail integral from $t$ to infinity. The same estimate sends that tail to zero, proving the [scattering from a finite Strichartz norm](../../../../../../scattering-from-a-finite-strichartz-norm.md) conclusion

$$
\|u(t)-S(t)u_\infty\|_2\longrightarrow0.
$$

## ↑ Ancestors (11)

1. [7](../7.md)
2. [1](../../1.md)
3. [Paper 154](../../../paper-154-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
