<h1 id="3/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The sources are independent odd [Grassmann variables](../../../../../../grassmann-variable.md) and anticommute with the [Dirac field](../../../../../../dirac-field.md). Use $K=\gamma^a\partial_a+M$ and the same mostly-plus [gamma matrices](../../../../../../gamma-matrices.md) and [Dirac adjoint](../../../../../../dirac-adjoint.md) as in the interaction calculation. The inverse $K_F^{-1}$ is selected with vacuum [Feynman i-epsilon prescription](../../../../../../feynman-i-epsilon-prescription.md) boundary conditions. With integral kernels and spinor contractions understood, the exponent can be completed to a square:

$$
\bar\psi K\psi+\bar\psi J+\bar J\psi
=(\bar\psi+\bar J K_F^{-1})K(\psi+K_F^{-1}J)
-\bar J K_F^{-1}J.
$$

Translations preserve the [Berezin integral](../../../../../../berezin-integral.md), so the [Gaussian generating functional for a Dirac field](../../../../../../gaussian-generating-functional-for-a-dirac-field.md) is

$$
\boxed{Z[J,\bar J]=Z[0,0]\exp\!\left[-i\int d^4x\,d^4y\,
\bar J(x)K_F^{-1}(x,y)J(y)\right]}.
$$

The positions of the sources matter. To extract the [Dirac propagator](../../../../../../dirac-propagator.md), use a left [Grassmann derivative](../../../../../../grassmann-derivative.md) with respect to $\bar J_\alpha(x)$ followed by a right [Grassmann derivative](../../../../../../grassmann-derivative.md) with respect to $J_\beta(y)$:

$$
S_{F,\alpha\beta}(x,y)
=-\frac1{Z[0,0]}\left.
\left(\frac{\delta_L Z}{\delta\bar J_\alpha(x)}\right)
\frac{\overleftarrow\delta}{\delta J_\beta(y)}\right|_{J=\bar J=0}
=i(K_F^{-1})_{\alpha\beta}(x,y).
$$

The leading minus sign removes the two insertion factors $i^2$. It can also be checked by differentiating the quadratic source exponential: its ordered second derivative is $-iZ[0,0]K_F^{-1}$.

For the [Fourier transform](../../../../../../fourier-transform.md) $e^{ip\cdot(x-y)}$, $K(p)=i\not p+M$ and the [Clifford algebra](../../../../../../clifford-algebra.md) gives

$$
(i\not p+M)(M-i\not p)=p^2+M^2.
$$

Therefore

$$
\boxed{S_F(x,y)=\int\frac{d^4p}{(2\pi)^4}\,e^{ip\cdot(x-y)}
\frac{i(M-i\not p)}{p^2+M^2-i0}}.
$$

This equals $\langle0|T\psi(x)\bar\psi(y)|0\rangle$. The fermionic [time ordering](../../../../../../time-ordering.md) is explicitly

$$
T\psi_\alpha(x)\bar\psi_\beta(y)
=\theta(x^0-y^0)\psi_\alpha(x)\bar\psi_\beta(y)
-\theta(y^0-x^0)\bar\psi_\beta(y)\psi_\alpha(x),
$$

with the minus sign supplied by exchanging odd fields. The poles put positive [energy](../../../../../../energy.md) forward in time and negative [energy](../../../../../../energy.md) backward, which is the [antiparticle](../../../../../../antiparticle.md) contribution. Finally, $K_xS_F(x,y)=iI\delta^{(4)}(x-y)$ checks the numerator and overall sign. All formulas are distributional limits with the indicated boundary prescription.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [3](../../3.md)
3. [Paper 40](../../../paper-40-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
