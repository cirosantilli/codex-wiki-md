<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For an [alpha-quenching rotating wave](../../../../../../alpha-quenching-rotating-wave.md), write the four complex fields as constant amplitudes times $e^{i\omega t}$, with $\omega$ real. The squared toroidal amplitudes are then constant, so the [algebraic alpha quenching](../../../../../../algebraic-alpha-quenching.md) coefficients are constant on the orbit. Assume $\Omega\ne0$. With $\epsilon_2=0$, the toroidal equations determine

$$
A_1=\frac{\omega-i}{\Omega}B_1,\qquad
A_2=-\frac{\omega-i}{\Omega}B_2.
$$

Substitution in the potential equations gives the amplitude [eigenvalue](../../../../../../eigenvalue.md) problem

$$
\frac{2\omega-i(1-\omega^2)}{\Omega}
\begin{pmatrix}B_1\\B_2\end{pmatrix}
=
\begin{pmatrix}\alpha_0-p|B_1|^2&\epsilon_1\\
\epsilon_1&\alpha_0-p|B_2|^2\end{pmatrix}
\begin{pmatrix}B_1\\B_2\end{pmatrix}.
$$

The matrix is real symmetric, hence [Hermitian](../../../../../../hermitian-operator.md), and every one of its [eigenvalues](../../../../../../eigenvalue.md) is real. For a nonzero amplitude vector this forces $1-\omega^2=0$. Thus **every nonzero rotating wave of this form has**

$$
\boxed{\omega=\pm1}.
$$

Set $a=\alpha_0-2\omega/\Omega$. In the dipole subspace $B_2=-B_1$ and $A_2=A_1$; in the quadrupole subspace $B_2=B_1$ and $A_2=-A_1$. The amplitude equations give

$$
\boxed{R_d^2=|B_1|^2=|B_2|^2=\frac{a-\epsilon_1}{p}},\qquad
\boxed{R_q^2=|B_1|^2=|B_2|^2=\frac{a+\epsilon_1}{p}}.
$$

These are nonzero waves exactly when the respective squared amplitude is positive. A common constant phase of $B_1,B_2$ is arbitrary, and $|A_j|^2=2|B_j|^2/\Omega^2$. In particular, choosing $\omega=\operatorname{sgn}\Omega$, both parities exist once $\alpha_0>2/|\Omega|+|\epsilon_1|$. The other frequency sign is also algebraically possible whenever its positivity conditions hold; existence alone says nothing about stability of that branch.

There is a genuine sign qualification in the polynomial [alpha quenching](../../../../../../algebraic-alpha-quenching.md) law. It subtracts $p|B|^2$ independently of the sign of $\alpha_0$. Thus a sufficiently large positive $\alpha_0$ gives the intended waves, but a sufficiently large negative $\alpha_0$ makes every displayed squared amplitude negative for both frequency signs. For example, with $\Omega=1$, $\epsilon_1=0$, $\alpha_0=-M$ and $M>2$, neither $(-M-2)/p$ nor $(-M+2)/p$ is nonnegative. **Large $|\alpha_0\Omega|$ alone is insufficient as printed; positive alpha, or the exact amplitude-positivity conditions above, is required.** A sign-preserving quenching prescription would be a different model.

For the [unequal-hemisphere dynamo rotating wave](../../../../../../unequal-hemisphere-dynamo-rotating-wave.md), first take $\epsilon_1\ne0$. The real symmetric matrix above has distinct [eigenvalues](../../../../../../eigenvalue.md) because its off-diagonal entry is nonzero. Its [eigenvector](../../../../../../eigenvector.md) is real up to a common complex phase, so choose $B_1=b_1$, $B_2=b_2$ real. The amplitude equations reduce to

$$
(a-pb_1^2)b_1+\epsilon_1b_2=0,\qquad
(a-pb_2^2)b_2+\epsilon_1b_1=0.
$$

Multiplying the first equation by $b_2$, the second by $b_1$, and subtracting gives

$$
(b_1^2-b_2^2)(pb_1b_2+\epsilon_1)=0.
$$

For unequal magnitudes, therefore, $b_1b_2=-\epsilon_1/p$. Neither amplitude can vanish. Multiplying the first amplitude equation by $b_1$ then shows $apb_1^2-p^2b_1^4-\epsilon_1^2=0$. Equivalently,

$$
 b_1^2+b_2^2=\frac ap,\qquad b_1^2b_2^2=\frac{\epsilon_1^2}{p^2}.
$$

The two distinct positive roots exist precisely when $a>2|\epsilon_1|$. This constructs the desired solutions explicitly:

$$
\boxed{b_{1,2}^2=\frac{a\pm\sqrt{a^2-4\epsilon_1^2}}{2p},\qquad
b_1b_2=-\frac{\epsilon_1}{p},\qquad a>2|\epsilon_1|}.
$$

Choose $b_1$ to be either square root of the first value, and set $b_2=-\epsilon_1/(pb_1)$; substituting verifies both amplitude equations. Interchanging the two roots gives the hemisphere-exchanged companion. The hinted choice $\omega=1$ therefore requires $\alpha_0-2/\Omega>2|\epsilon_1|$. At equality the magnitudes coincide, so it is not an asymmetric solution. For $\epsilon_1>0$ the amplitudes have opposite signs and meet the dipole branch at equality; for $\epsilon_1<0$ they have the same sign and meet the quadrupole branch.

If $\epsilon_1=0$, the hemispheres decouple. An asymmetric rotating wave instead has one hemisphere inactive and the other with $|B|^2=a/p>0$. If both hemispheres are active their magnitudes must be equal, although their relative phase is arbitrary. If $\Omega=0$, the toroidal equations simply give $\dot B_j=-B_j$, so no nonzero common-frequency rotating wave exists.

The unequal-amplitude solutions describe **a periodically reversing dynamo concentrated more strongly in one hemisphere**, with $|A_1|\ne|A_2|$ following from $|A_j|=\sqrt2|B_j|/|\Omega|$. Both $B_d=(B_1-B_2)/2$ and $B_q=(B_1+B_2)/2$ are nonzero, so the field combines the two [dipole and quadrupole parity in a mean-field dynamo](../../../../../../dipole-and-quadrupole-parity-in-a-mean-field-dynamo.md) classes rather than belonging to either one. Equatorial reflection exchanges the two companion solutions. The model can therefore break hemispheric symmetry without asymmetric input parameters. This construction proves existence; nonlinear stability would require an additional perturbation calculation.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 68](../../../paper-68-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
