<h1 id="2/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

First fix the [propagator kernels in a positive-sign Gaussian generating functional](../../../../../propagator-kernels-in-a-positive-sign-gaussian-generating-functional.md). From its scalar exponent, $i^{-2}\delta^2Z_0/\delta J\delta J$ gives the contraction $D(x-y)=-i\Delta(x-y)$. The fermionic insertion rules similarly give $F(x-y)=\langle T\psi(x)\bar\psi(y)\rangle_0=-iS(x-y)$, writing $S$ for the kernel labelled $S_F$ in that exponent. Thus the kernels in the question do not already include the factors of $i$ in the actual time-ordered contractions.

At order $g^2$, expand the interaction operator to its second term, or equivalently apply [Wick's theorem](../../../../../wick-s-theorem.md) to

$$
\frac{(ig)^2}{2}\int d^4x\,d^4y\,
\left\langle T\phi(x_a)\phi(y_a)
\phi(x)\bar\psi(x)\psi(x)\phi(y)\bar\psi(y)\psi(y)\right\rangle_0.
$$

For a connected contribution, the external scalar insertions attach to different interaction points. The two assignments are equal after exchanging $x,y$ and cancel $1/2$. The connected fermionic contraction is

$$
\left\langle T\bar\psi_\alpha(x)\psi_\alpha(x)
\bar\psi_\beta(y)\psi_\beta(y)\right\rangle_{0,c}
=-F_{\alpha\beta}(x-y)F_{\beta\alpha}(y-x)
=-\operatorname{tr}[F(x-y)F(y-x)].
$$

The minus sign is the [closed fermion loop sign](../../../../../closed-fermion-loop-sign.md). The alternative pairing gives two separate [fermion](../../../../../fermion.md) tadpoles and belongs to disconnected external components, not the requested connected function. A free external scalar line multiplying a [vacuum](../../../../../vacuum.md) graph also cancels in the normalized result.

Combining $(ig)^2=-g^2$ with the loop minus sign gives

$$
G^{(2)}_c\big|_{g^2}=g^2\int d^4x\,d^4y\,
D(x_a-x)D(y_a-y)\operatorname{tr}[F(x-y)F(y-x)].
$$

There are four contractions, so replacing $D=-i\Delta$ and $F=-iS$ introduces $(-i)^4=1$. Therefore

$$
\boxed{G^{(2)}_c\big|_{g^2}=g^2\int d^4x\,d^4y\,
\Delta(x_a-x)\Delta(y_a-y)\operatorname{tr}[S(x-y)S(y-x)].}
$$

This is the fermion-loop diagram in the last panel of [i](../../../1/b/i.md). The [trace](../../../../../matrix-trace.md) contracts [spinor](../../../../../spinor.md) indices around the loop; it is not an additional degeneracy factor. A convention using physical contractions directly obtains the preceding formula in $D,F$ with the same coefficient. Mixing one convention's Gaussian kernels with another's insertion factors would change its apparent signs.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [2](../../../2.md)
4. [2018](../../../../2018-split.md)
5. [Past exam of the advanced quantum field theory for particle physics course of the University of Oxford](../../../../split.md)
6. [Advanced quantum field theory for particle physics course of the University of Oxford](../../../../../advanced-quantum-field-theory-for-particle-physics-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Mathematical and theoretical physics course of the University of Oxford](../../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
