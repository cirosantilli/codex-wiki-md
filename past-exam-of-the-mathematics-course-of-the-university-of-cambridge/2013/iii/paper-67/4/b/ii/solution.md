<h1 id="4/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

**The ordinary [Fourier transform](../../../../../../../fourier-transform.md) does not exist.** There is a real [simple pole](../../../../../../../simple-pole.md) at $x=-1$, with

$$
\frac1{1+x^3}=\frac1{3(x+1)}+O(1)\quad(x\to-1).
$$

The two separate improper integrals diverge logarithmically. Thus no ordinary large-$k$ expansion is defined under the stated integral convention. A [Cauchy principal value](../../../../../../../cauchy-principal-value.md) or a contour prescription would be additional data, and must be stated rather than silently introduced.

For completeness, the symmetric [Cauchy principal value](../../../../../../../cauchy-principal-value.md) has a precise answer. The real [pole](../../../../../../../pole.md) contributes the [principal-value Fourier transform of a real pole](../../../../../../../principal-value-fourier-transform-of-a-real-pole.md)

$$
\mathcal F\!\left(\operatorname{PV}\frac1{3(x+1)}\right)=-\frac{i\pi}{3}\operatorname{sgn}(k)e^{ik}.
$$

The other [poles](../../../../../../../pole.md) are $z_\pm=(1\pm i\sqrt3)/2$ with [residues](../../../../../../../residue.md) $r_\pm=1/(3z_\pm^2)=(-1\mp i\sqrt3)/6$. For $k>0$, close the [contour integration](../../../../../../../contour-integration.md) in the lower half-plane, with clockwise orientation. The nonreal [pole](../../../../../../../pole.md) contributes $-2\pi i r_-e^{-ikz_-}$, while the real principal-value [pole](../../../../../../../pole.md) supplies the half-residue above. For $k<0$, the upper-half-plane contour gives the conjugate result. With $s=\operatorname{sgn}(k)$, the exact principal-value formula for $k\ne0$ is

$$
\boxed{\widehat f_{\rm PV}(k)=-\frac{i\pi}{3}s e^{ik}+\frac\pi3(\sqrt3+is)\exp\left(-\frac{\sqrt3}{2}|k|-\frac i2k\right)}.
$$

These are its two nonzero asymptotic contributions: a nondecaying oscillatory real-pole term and an exponentially small complex-pole term. There is no second nonzero inverse-power term. This formula is qualified by the principal-value choice; it is not the ordinary transform requested in the statement.

Other prescriptions change the leading term. For example, replacing the real [pole](../../../../../../../pole.md) by its upper or lower boundary value changes the distribution by $\mp i\pi\delta(x+1)/3$, and hence changes the transform by $\mp i\pi e^{ik}/3$. This demonstrates why a [pole](../../../../../../../pole.md) prescription is essential. The smooth [Taylor series](../../../../../../../taylor-series.md) at the origin alone would miss the decisive real-pole contribution.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [4](../../../4.md)
4. [Paper 67](../../../../paper-67-split.md)
5. [Iii](../../../../split.md)
6. [2013](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
