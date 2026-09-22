<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

There are **three independent nonfactorized [momentum integrals](../../../../momentum-space-integral.md)**, namely a [tadpole integral](../../../../tadpole-integral.md), the three-line [sunset diagram](../../../../sunset-diagram.md) integral, and the [five-line banana integral](../../../../five-line-banana-integral.md). The six displayed [Feynman diagrams](../../../../feynman-diagram.md) involve **six complete integral expressions**:

$$
\boxed{T,\quad T^2,\quad B_3(P),\quad T B_3(P),\quad T^2B_3(P),\quad B_5(P).}
$$

The distinction between independent building blocks and their products removes an ambiguity in counting “different momentum integrals”. For the strict divergent-[wave-function renormalization](../../../../wave-function-renormalization.md) interpretation of [ii](../c/ii.md), the graphs in [c](../c.md) reduce to $T,T^2,B_5$, comprising **three full integral expressions and two independent nonfactorized building blocks**.

Make a [Wick rotation](../../../../wick-rotation.md) and use $m>0$ to separate [ultraviolet divergences](../../../../ultraviolet-divergence.md) from [infrared divergences](../../../../infrared-divergence.md). Write $D_E(k)=1/(k^2+m^2)$, and let $T,B_r(P)$ be the Euclidean versions of the integrals above, with their harmless overall factors of $i$ removed. A spherical [ultraviolet cutoff](../../../../ultraviolet-cutoff.md) gives

$$
T_\Lambda=\frac1{2\pi^2}\int_0^\Lambda\frac{k^2\,dk}{k^2+m^2}
=\frac1{2\pi^2}\left[\Lambda-m\arctan(\Lambda/m)\right]
=\frac{\Lambda}{2\pi^2}-\frac{m}{4\pi}+O(\Lambda^{-1}).
$$

Thus the one-vertex quartic graph is linearly divergent, and the one-vertex sextic graph is quadratically divergent as $T_\Lambda^2$.

For the other two building blocks, the spatial [Fourier transform](../../../../fourier-transform-split.md) is especially transparent. The three-dimensional Euclidean [scalar propagator](../../../../scalar-propagator.md) is

$$
G(x)=\int\frac{d^3k}{(2\pi)^3}\frac{e^{ik\cdot x}}{k^2+m^2}
=\frac{e^{-m|x|}}{4\pi|x|}.
$$

The [convolution theorem](../../../../convolution-theorem.md) converts the $r$ parallel lines into $G(x)^r$. Angular integration gives, with a short-distance cutoff $a=\Lambda^{-1}$,

$$
B_r^{(a)}(P)=\frac{4\pi}{(4\pi)^r}\int_a^\infty
\rho^{2-r}e^{-rm\rho}\frac{\sin(P\rho)}{P\rho}\,d\rho,
\qquad P=|P_E|.
$$

This is a different convenient [cutoff regularization](../../../../cutoff-regularization.md) for the connected block; power-divergent coefficients depend on the cutoff convention, whereas the conclusions about powers and the presence of a kinetic logarithm do not. The [sinc function](../../../../sinc-function.md) is understood to be $1$ at $P=0$.

For $r=3$, the integrand starts as $\rho^{-1}+O(1)$, so

$$
B_3^{(a)}(P)=\frac1{16\pi^2}\log\frac1{ma}+O(1).
$$

Its divergent part is independent of external [momentum](../../../../momentum-split.md). In particular,

$$
B_3(P)-B_3(0)=\frac1{16\pi^2}\int_0^\infty\frac{e^{-3m\rho}}\rho
\left[\frac{\sin(P\rho)}{P\rho}-1\right]d\rho
=-\frac{P^2}{864\pi^2m^2}+O(P^4).
$$

The finite difference and its finite derivative show why the pure three-line [sunset diagram](../../../../sunset-diagram.md) does not need a divergent [wave-function renormalization](../../../../wave-function-renormalization.md) in three dimensions.

For $r=5$, the small-distance [Taylor expansion](../../../../taylor-expansion.md) is

$$
\rho^{-3}e^{-5m\rho}\frac{\sin(P\rho)}{P\rho}
=\rho^{-3}-5m\rho^{-2}
+\left(\frac{25m^2}{2}-\frac{P^2}{6}\right)\rho^{-1}+O(1).
$$

Consequently

$$
\boxed{B_5^{(a)}(P)\big|_{\mathrm{div}}
=\frac1{256\pi^4}\left[\frac1{2a^2}-\frac{5m}{a}
+\left(\frac{25m^2}{2}-\frac{P^2}{6}\right)\log\frac1{ma}\right].}
$$

In particular, the nonzero $P^2\log\Lambda$ term requires a genuine divergent [wave-function renormalization](../../../../wave-function-renormalization.md), in addition to the [mass counterterm](../../../../mass-counterterm.md). The coefficients here refer to the displayed position-space cutoff and have not included [Feynman-diagram symmetry factors](../../../../feynman-diagram-symmetry-factor.md) or [bare couplings](../../../../bare-coupling.md).

The comparison with the [superficial degree of divergence](../../../../superficial-degree-of-divergence.md) is

$$
\begin{array}{c|c|c|c}
\text{vertices and integral}&(n_4,n_6)&\omega&\text{leading unrenormalized growth}\\\hline
4:\ T&(1,0)&1&\Lambda\\
6:\ T^2&(0,1)&2&\Lambda^2\\
4,4:\ B_3&(2,0)&0&\log\Lambda\\
4,6:\ TB_3&(1,1)&1&\Lambda\log\Lambda\\
6,6:\ T^2B_3&(0,2)&2&\Lambda^2\log\Lambda\\
6,6:\ B_5&(0,2)&2&\Lambda^2
\end{array}
$$

Thus the actual leading power agrees with $\omega$ in every case. The additional logarithms in products come from [ultraviolet subdivergences](../../../../ultraviolet-subdivergence.md), which uniform [power counting](../../../../power-counting-in-quantum-field-theory.md) alone does not resolve.

For $TB_3$ and $T^2B_3$, differentiation with respect to $P^2$ removes the logarithmic divergence of $B_3$, but leaves divergent factors $T$ or $T^2$ multiplying a finite, nonpolynomial function of $P^2$. These are subdivergent contributions, not new nonlocal [counterterms](../../../../counterterm.md): subtracting each [tadpole diagram](../../../../tadpole-diagram.md) subdivergence and the momentum-independent $B_3$ subdivergence removes them. For example, in a factorized subtraction scheme $TB_3\mapsto(T-T_{\mathrm{div}})(B_3-B_{3,\mathrm{div}})$, and likewise for $T^2B_3$. The remaining $B_5$ kinetic logarithm explains the strict interpretation in [ii](../c/ii.md). A [dimensional regularization](../../../../dimensional-regularization.md) scheme can suppress power divergences; it does not invalidate this cutoff-based comparison with $\omega$.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [3](../../3.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the quantum field theory course of the University of Oxford](../../../split.md)
5. [Quantum field theory course of the University of Oxford](../../../../quantum-field-theory-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
