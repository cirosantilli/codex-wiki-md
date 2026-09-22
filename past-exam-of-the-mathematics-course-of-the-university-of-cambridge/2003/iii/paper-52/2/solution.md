<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

In the usual smooth localized finite-energy class, the positive potential requires $|\phi|\to1$ at infinity and the [gauge covariant derivative](../../../../../gauge-covariant-derivative.md) tends to zero there. On a sufficiently large circle write $\phi\simeq e^{i\chi}$ locally. Then the tangential [gauge potential](../../../../../gauge-field.md) approaches $d\chi$. The normalized Higgs phase defines a continuous map $S^1_\infty\to U(1)$ with integer [winding number](../../../../../winding-number.md)

$$
\boxed{N=\frac1{2\pi}\oint d\chi=\frac1{2\pi}\int_{\mathbb R^2}B\,d^2x\in\mathbb Z.}
$$

The second equality is [Stokes theorem](../../../../../stokes-theorem.md) with the chosen orientation and $D_j=\partial_j-ia_j$. Suitable decay makes the integrated covariant-derivative error vanish. Thus [magnetic flux quantization of an Abelian Higgs vortex](../../../../../magnetic-flux-quantization-of-an-abelian-higgs-vortex.md) labels disconnected boundary sectors. This uses the standard continuous vacuum asymptotics, not a claim that bare integral finiteness alone supplies every pointwise boundary limit.

A nonzero winding requires zeros of the complex [Higgs field](../../../../../higgs-field.md) somewhere inside: a nowhere-zero field on the whole disk would extend its normalized boundary map and make its winding zero. For isolated zeros the signed local indices sum to $N$. For arbitrary configurations, vortex-antivortex pairs may add zeros without changing $N$, so $|N|$ need not count all unsigned zeros.

The [critical coupling](../../../../../critical-coupling.md) relates the charge to a minimum energy. Set $j_i=\operatorname{Im}(\bar\phi D_i\phi)$. The covariant derivative commutator $[D_1,D_2]\phi=-iB\phi$ gives

$$
|D_1\phi|^2+|D_2\phi|^2=|(D_1+iD_2)\phi|^2+B|\phi|^2+\partial_1j_2-\partial_2j_1.
$$

Discarding its vanishing boundary integral and completing the magnetic square yields

$$
E=\int\left\{\frac12|(D_1+iD_2)\phi|^2+\frac12\left[B-\frac{1-|\phi|^2}{2}\right]^2\right\}d^2x+\frac12\int B\,d^2x.
$$

For positive $N$, the [Bogomolny vortex equations](../../../../../bogomolny-vortex-equation.md) are $(D_1+iD_2)\phi=0$ and $B=(1-|\phi|^2)/2$. Reverse both signs for negative charge. Hence

$$
\boxed{E\ge\pi|N|.}
$$

Critical-coupling vortex solutions attain this bound; their energy depends only on $|N|$. Positive-charge solutions have $N$ zeros counted with multiplicity, and their positions provide $2N$ real coordinates on the [Abelian Higgs vortex moduli space](../../../../../abelian-higgs-vortex-moduli-space.md). Coincident zeros are allowed. Position variations leave the static minimum energy unchanged, expressing the absence of static forces among same-sign Bogomolny vortices. The sign of $N$ reverses flux and orientation. Topology alone does not determine an arbitrary field's profile or full energy: the zero-charge vacuum has energy zero, while nonvacuum configurations in the same sector can have positive energy.

For the given radial ansatz, $a_\theta$ is the coordinate one-form coefficient: the [gauge potential](../../../../../gauge-field.md) is $a(r)d\theta$, and the orthonormal azimuthal component is $a(r)/r$. Thus $B=a'(r)/r$, consistently with the printed energy. Since $h(\infty)=1$, the phase $e^{i\theta}$ has winding one; equivalently $a(0)=0$, $a(\infty)=1$ gives

$$
\boxed{N=1,\qquad\int B\,d^2x=2\pi[a(\infty)-a(0)]=2\pi.}
$$

For the trial functions all energy is inside $0<r<r_0$. Their four contributions to $E/\pi$ are

$$
\begin{aligned}
\text{magnetic: }&\int_0^{r_0}\frac{(2r/r_0^2)^2}{r^2}r\,dr=\frac2{r_0^2},\\
\text{radial gradient: }&\int_0^{r_0}\frac1{r_0^2}r\,dr=\frac12,\\
\text{angular gradient: }&\int_0^{r_0}\frac{(1-r^2/r_0^2)^2}{r_0^2}r\,dr=\frac16,\\
\text{potential: }&\frac14\int_0^{r_0}(1-r^2/r_0^2)^2r\,dr=\frac{r_0^2}{24}.
\end{aligned}
$$

Therefore the [compact-core variational estimate for an Abelian Higgs vortex](../../../../../compact-core-variational-estimate-for-an-abelian-higgs-vortex.md) is

$$
\boxed{E(r_0)=\pi\left(\frac2{r_0^2}+\frac23+\frac{r_0^2}{24}\right).}
$$

Writing $s=r_0^2>0$, the derivative is $-2/s^2+1/24$, and the energy diverges at both ends of the $s$ range. The unique global minimum is

$$
\boxed{r_0^4=48,\quad r_0^2=4\sqrt3,\quad E_{\rm trial,min}=\pi\left(\frac23+\frac1{\sqrt3}\right)\simeq1.24402\pi.}
$$

The magnetic and potential energies agree at this optimum, as required by radial scale balance. The piecewise fields are continuous with square-integrable first derivatives; their derivative jumps do not create an additional surface energy. They are trial fields, not exact solutions. Their optimized energy is an upper-bound estimate, about 24.4% above the exact critical one-vortex energy $\pi$.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 52](../../paper-52-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
