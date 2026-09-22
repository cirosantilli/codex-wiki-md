<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Split the free [scalar field](../../../../../../scalar-field.md) into its annihilation part $\phi^{(+)}$ and creation part $\phi^{(-)}$. [Normal ordering](../../../../../../normal-ordering.md) moves every creation operator to the left of every annihilation operator, without adding the commutators produced by that rearrangement. For two fields,

$$
:\phi(x)\phi(y):=
\phi^{(-)}(x)\phi^{(-)}(y)+\phi^{(-)}(x)\phi^{(+)}(y)
+\phi^{(-)}(y)\phi^{(+)}(x)+\phi^{(+)}(x)\phi^{(+)}(y).
$$

Its vacuum expectation is zero. [Time ordering](../../../../../../time-ordering.md) instead places the field at the later time on the left:

$$
T\{\phi(x)\phi(y)\}
=\theta(x^0-y^0)\phi(x)\phi(y)+\theta(y^0-x^0)\phi(y)\phi(x).
$$

The equal-time convention is immaterial away from coincident singularities; these expressions are understood as [operator-valued distributions](../../../../../../operator-valued-distribution.md).

The only nonzero vacuum contraction uses $a_{\mathbf p}a^\dagger_{\mathbf q}$. The oscillator [commutator](../../../../../../commutator.md) therefore gives the [Wightman function](../../../../../../wightman-function.md)

$$
W(x-y)=\langle0|\phi(x)\phi(y)|0\rangle
=\int\frac{d^3p}{(2\pi)^3}\frac{e^{-iE_{\mathbf p}(x^0-y^0)+i\mathbf p\cdot(\mathbf x-\mathbf y)}}{2E_{\mathbf p}}.
$$

Put $\tau=x^0-y^0$ and $\mathbf r=\mathbf x-\mathbf y$. Combining the two time orders, and reversing $\mathbf p$ in the second when necessary, gives

$$
\Delta_F(\tau,\mathbf r)
=\int\frac{d^3p}{(2\pi)^3}\frac{e^{i\mathbf p\cdot\mathbf r-iE_{\mathbf p}|\tau|}}{2E_{\mathbf p}}.
$$

To recover the four-dimensional [Fourier transform](../../../../../../fourier-transform.md), use the [Feynman i-epsilon prescription](../../../../../../feynman-i-epsilon-prescription.md) in the energy variable:

$$
\int\frac{dp^0}{2\pi}\frac{i e^{-ip^0\tau}}{(p^0)^2-E_{\mathbf p}^2+i0}
=\frac{e^{-iE_{\mathbf p}|\tau|}}{2E_{\mathbf p}}.
$$

The positive-energy pole lies just below the real axis, and the negative-energy pole just above it. For $\tau>0$, close below clockwise: the residue at $E_{\mathbf p}-i0$ is $i e^{-iE_{\mathbf p}\tau}/(2E_{\mathbf p})$, and the clockwise factor $-i$ after dividing by $2\pi$ gives the required positive coefficient. For $\tau<0$, close above counterclockwise: the residue at $-E_{\mathbf p}+i0$ is $-i e^{iE_{\mathbf p}\tau}/(2E_{\mathbf p})$, and the factor $+i$ gives the other time order. Equivalently the energy contour passes above the positive-energy pole and below the negative-energy pole. Hence

$$
\boxed{\Delta_F(x-y)=\lim_{\epsilon\downarrow0}
\int\frac{d^4p}{(2\pi)^4}\frac{i e^{-ip\cdot(x-y)}}{p^2-\mu^2+i\epsilon}.}
$$

The limit is distributional. The [scalar Feynman propagator pole prescription](../../../../../../scalar-feynman-propagator-pole-prescription.md) is essential; omitting it from the denominator must be accompanied by the specified contour.

Finally, moving the annihilation part of $\phi(x)$ past the creation part of $\phi(y)$ gives

$$
\phi(x)\phi(y)=:\phi(x)\phi(y):+W(x-y)\mathbf1.
$$

The normal-ordered two-field product is symmetric in $x,y$, because the two creation parts commute and the two annihilation parts commute. Applying the two time orders thus proves the [two-field scalar Wick identity](../../../../../../two-field-scalar-wick-identity.md)

$$
\boxed{T\{\phi(x)\phi(y)\}=:\phi(x)\phi(y):+\Delta_F(x-y)\mathbf1.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 48](../../../paper-48-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
