<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

A degenerate [optical parametric amplifier](../../../../optical-parametric-amplifier.md) sends a strong pump at $2\omega$ through a phase-matched second-order nonlinear medium, creating pairs in a selected mode near $\omega$. With the pump treated classically and undepleted, the effective interaction is quadratic in the mode's [creation and annihilation operators](../../../../creation-and-annihilation-operators.md). Vacuum input evolves into an [optical squeezed vacuum](../../../../optical-squeezed-vacuum.md); the pump phase fixes the quiet [optical quadrature](../../../../optical-quadrature.md). A cavity enhances the interaction below oscillation threshold. [balanced homodyne detection](../../../../balanced-homodyne-detection.md) compares this [optical quadrature](../../../../optical-quadrature.md)'s noise with the blocked-signal vacuum reference; phase locking, detector balance, electronic-noise measurement and loss calibration distinguish squeezing from an instrumental noise reduction. A primary cavity experiment observed below-vacuum noise by degenerate down conversion and balanced homodyne readout.[1986, abstract: cavity down conversion and homodyne noise reduction](../../../../generation-of-squeezed-states-by-parametric-down-conversion-by-ling-an-wu-and-others.md)

Use $S(r)=\exp[\tfrac r2(a^2-a^{\dagger2})]$, so $S^\dagger aS=a\cosh r-a^\dagger\sinh r$. Write $s=\sinh^2r$, $c=\cosh r$ and $N=a^\dagger a$. Vacuum expectations then give

$$
\boxed{\langle N\rangle=s},\qquad
\langle a^2\rangle=-\sinh r\cosh r.
$$

Pair creation makes the mean field zero while the mean [photon number](../../../../photon-number.md) is positive. Expanding the transformed ladder operators in the vacuum gives the [squeezed-vacuum photon-number moments](../../../../squeezed-vacuum-photon-number-moments.md): $\langle N(N-1)\rangle=3s^2+s$ and $\langle N^2\rangle=3s^2+2s$; equivalently $\operatorname{Var}N=2s(s+1)$.

The vectors produced by [photon addition](../../../../photon-addition.md) and [photon subtraction](../../../../photon-subtraction.md) in the paper are not normalized. Their squared norms are $s+1$ and $s$, respectively. A particularly direct evaluation is

$$
a^\dagger S(r)|0\rangle=cS(r)|1\rangle,\qquad
aS(r)|0\rangle=-\sinh r\,S(r)|1\rangle.
$$

Both successful operations therefore prepare the same [squeezed one-photon state](../../../../squeezed-one-photon-state.md), up to an overall phase, whenever subtraction has nonzero [probability](../../../../probability.md). Since $\langle1|S^\dagger NS|1\rangle=c^2+2s=1+3s$, the unnormalized moments are

$$
M_+=\langle\Psi_+|N|\Psi_+\rangle=(c^2+2s)c^2=(3s+1)(s+1),
\qquad M_-=\langle\Psi_-|N|\Psi_-\rangle=s(3s+1).
$$

**The printed photon-added formula equals $M_+$, not a normalized mean.** With its literal unnormalized convention, the corresponding subtraction result is $M_-$ and

$$
\boxed{M_+-M_-=1+3\sinh^2r>0.}
$$

This difference tends to one as $r\to0$ and grows as $\tfrac34e^{2r}$ for large positive $r$. Keeping this convention recovers the paper's requested expression without misidentifying it as a physical conditional mean.

For the [normalization of photon-added and photon-subtracted states](../../../../normalization-of-photon-added-and-photon-subtracted-states.md), divide by the squared norms to obtain actual conditional means:

$$
\boxed{\bar n_+=\frac{M_+}{s+1}=1+3s,
\qquad \bar n_-=\frac{M_-}{s}=1+3s,
\qquad \bar n_+-\bar n_-=0.}
$$

These equalities for subtraction require $s>0$. As $r\to0$ the normalized successful subtraction tends to $|1\rangle$, but its success [probability](../../../../probability.md) vanishes; exactly at $r=0$, $a|0\rangle=0$ gives no conditional state. At large $r$, both normalized means grow as $3e^{2r}/4$, while their difference remains zero.

For the [photon statistics of a squeezed vacuum](../../../../photon-statistics-of-a-squeezed-vacuum.md), the even-number [probabilities](../../../../probability.md) are

$$
p_{2m}=\frac{(2m)!}{2^{2m}(m!)^2}\frac{\tanh^{2m}r}{\cosh r},\qquad p_{2m+1}=0.
$$

After subtraction the normalized distribution is $p^-_n=(n+1)p_{n+1}/s$. It has only odd occupation and no vacuum component. [photon addition](../../../../photon-addition.md) gives $p^+_n=np_{n-1}/(s+1)$, identical here to $p^-_n$. The diagram uses normalized distributions with an explicitly chosen $r$, rather than treating the unnormalized moments as means.

<a id="2/image-original-normalized-even-squeezed-vacuum-and-odd-conditional-photon-number-distributions-with-raw-moment-and-mean-conventions-distinguished"></a>
![](../../../../past-exam-of-the-nonlinear-optics-and-quantum-states-of-light-course-of-the-university-of-cambridge/2014/paper-1-conditioned-photon-statistics.png)

**[Figure 2](#2/image-original-normalized-even-squeezed-vacuum-and-odd-conditional-photon-number-distributions-with-raw-moment-and-mean-conventions-distinguished). Original normalized even squeezed-vacuum and odd conditional photon-number distributions, with raw-moment and mean conventions distinguished**.

A subtraction event samples initial occupation with weight $n$, preferentially selecting the larger components before removing one [photon](../../../../photon.md). In general $\bar n_-=\langle N(N-1)\rangle/\langle N\rangle=\langle N\rangle-1+\operatorname{Var}N/\langle N\rangle$. Here the large [variance](../../../../variance-split.md) gives **$\bar n_--\langle N\rangle=1+2s>0$**. This [conditional photon-number bias](../../../../conditional-photon-number-bias.md) does not create [energy](../../../../energy-split.md) by removing a [photon](../../../../photon.md): the unconditional ensemble also includes the runs without a heralded event.

## ↑ Ancestors (13)

1. [2](../2.md)
2. [Paper 1](../../paper-1-split.md)
3. [2014](../../split.md)
4. [Past exam of the nonlinear Optics and Quantum States of Light course of the University of Cambridge](../../../split.md)
5. [Nonlinear Optics and Quantum States of Light course of the University of Cambridge](../../../../nonlinear-optics-and-quantum-states-of-light-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 4 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 4 of the natural sciences course of the University of Cambridge](../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)
