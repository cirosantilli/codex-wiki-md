<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Take $0<v<1$ and $\Gamma=(1-v^2)^{-1/2}$. The [Sine-Gordon kink-antikink scattering solution](../../../../../sine-gordon-kink-antikink-scattering-solution.md) tends to the same vacuum at both spatial ends and hence has zero net [topological charge](../../../../../topological-charge.md). At large $|t|$, the two transition centers, found by setting the magnitude of the inverse-tangent argument to one, obey

$$
\Gamma|x|=\Gamma v|t|-\log v+o(1).
$$

They are a [kink](../../../../../scalar-field-kink.md) and an [antikink](../../../../../antikink.md) moving with asymptotic speeds $\pm v$, with no outgoing radiation. Their left-right orientations interchange at the collision. To define the [soliton time delay](../../../../../soliton-time-delay.md), label a transmitted trajectory by its preserved [rapidity](../../../../../rapidity.md) rather than its left-right position. The right-moving asymptotes are

$$
x_{\rm in}=vt+\frac{\log v}{\Gamma},\qquad x_{\rm out}=vt-\frac{\log v}{\Gamma}.
$$

After restoring physical lengths, the forward shift is $\Delta X=-2\log v/(m\Gamma)>0$. The arrival-time difference is therefore

$$
\boxed{\Delta T=-\Delta X/v=\frac{2\log v}{m\Gamma v}=\frac{2\log\tanh(\theta/2)}{m\sinh(\theta/2)}<0,\qquad v=\tanh(\theta/2).}
$$

This is a time advance relative to the extrapolated incoming free motion.

**The semiclassical scattering phase.** For an outgoing energy wave packet with full [S-matrix](../../../../../s-matrix.md) phase $S=e^{i\delta(E)}$, [stationary phase](../../../../../stationary-phase-method.md) in $e^{-iET+i\delta(E)}$ shifts its arrival time by $d\delta/dE$. The [full S-matrix phase from a classical soliton delay](../../../../../full-s-matrix-phase-from-a-classical-soliton-delay.md) uses the paper's $\delta$, twice the phase in a convention $S=e^{2i\delta_{\rm pw}}$. In the center-of-momentum frame, $E=2\mathcal M_K\cosh(\theta/2)$, so $dE/d\theta=\mathcal M_K\sinh(\theta/2)$. It follows that

$$
\boxed{\frac{d\delta_{\rm sc}}{d\theta}=\frac{2\mathcal M_K}{m}\log\tanh(\theta/2).}
$$

The literal PDF normalization gives $\mathcal M_K=8m/\beta$ and consequently

$$
\boxed{\delta_{\rm literal}(\theta)=\delta_{\rm literal}(0)+\frac{16}{\beta}\int_0^\theta\log\tanh(u/2)du.}
$$

The integrable logarithmic singularity at zero causes no divergence of this phase difference. With the intended standard angular-field prefactor $m^2/\beta^2$, the result is instead

$$
\boxed{\delta_{\rm standard}(\theta)=\delta_{\rm standard}(0)+\frac{16}{\beta^2}\int_0^\theta\log\tanh(u/2)du.}
$$

The [soliton time delay](../../../../../soliton-time-delay.md) determines only phase differences, not an energy-independent constant or a choice of $2\pi$ branch. Keeping this distinction avoids an arbitrary high-energy subtraction.

**Bound-state poles.** Set $a_j=\pi j/N$. Each factor of the exact amplitude can be written $\cosh[(\theta-ia_j)/2]/\cosh[(\theta+ia_j)/2]$. Its denominator vanishes in the [physical rapidity strip](../../../../../physical-rapidity-strip.md) at

$$
\theta=iu_n,\qquad u_n=\pi(1-n/N),\qquad n=1,\ldots,N-1.
$$

The corresponding numerator is nonzero, and no other numerator cancels the pole. In the direct [kink](../../../../../scalar-field-kink.md)–[antikink](../../../../../antikink.md) fusion interpretation, analytically continue the constituent [rapidities](../../../../../rapidity.md) to $\pm iu_n/2$. Their momenta sum to $(2\mathcal M_K\cos(u_n/2),0)$, so the [relativistic bound-state mass from a rapidity pole](../../../../../relativistic-bound-state-mass-from-a-rapidity-pole.md) gives

$$
\boxed{\mathcal M_n=2\mathcal M_K\sin\frac{n\pi}{2N},\quad n=1,\ldots,N-1.}
$$

These neutral particles form the [Sine-Gordon breather spectrum at reflectionless couplings](../../../../../sine-gordon-breather-spectrum-at-reflectionless-couplings.md): there are $N-1$ breathers, none for $N=1$, and the putative $n=N$ state is at the unbound $2\mathcal M_K$ threshold. The amplitude fixes these ratios to the physical [kink](../../../../../scalar-field-kink.md) [mass](../../../../../mass.md); its [rapidity](../../../../../rapidity.md) dependence alone cannot fix the overall [mass](../../../../../mass.md) scale or a mass-renormalization prescription relating that [mass](../../../../../mass.md) to $m$.

It is important to distinguish direct and crossed interpretations rather than count every occurrence of a pole twice. [Crossing symmetry](../../../../../crossing-symmetry.md) sends $iu_n$ to $i(\pi-u_n)=iu_{N-n}$. At the original angle the momentum-difference invariant is $4\mathcal M_K^2\sin^2(u_n/2)=\mathcal M_{N-n}^2$, so the crossed interpretation exchanges the complementary member of the same tower. In particular the transmission residue alternates sign: direct evaluation of the remaining factors gives $\operatorname{Res}_{iu_n}S_T=i(-1)^n R_n$, $R_n>0$. Thus one must retain charge-channel/crossed-channel information, not reject every negative-imaginary transmission residue or declare an additional particle for a crossed pole. Direct and crossed locations coincide in the reflectionless pole set. The familiar $N=2$ case has one breather of [mass](../../../../../mass.md) $\sqrt2\mathcal M_K$ despite the negative-imaginary transmission residue; this diagonal reflectionless example is also displayed in [Castro-Alvaredo, Chen, Doyon and Hoogeveen, section 4.2](https://arxiv.org/pdf/1310.4779).

**Matching the exact phase.** For the [unwrapped reflectionless sine-Gordon transmission phase](../../../../../unwrapped-reflectionless-sine-gordon-transmission-phase.md), at real $\theta\geq0$ choose the continuous unwrapped branch with $\delta_N(0)=\pi N$. Then

$$
\boxed{\delta_N(\theta)=\pi N-2\sum_{j=1}^{N-1}\arctan\left[\tanh(\theta/2)\tan\frac{\pi j}{2N}\right].}
$$

Every factor has unit modulus, consistent with purely transmitting elastic scattering. Differentiating is simpler than integrating its complex logarithm:

$$
\delta_N'(\theta)=-\sum_{j=1}^{N-1}\frac{\sin(\pi j/N)}{\cosh\theta+\cos(\pi j/N)}.
$$

For fixed $\theta>0$ the sum becomes a [Riemann sum](../../../../../riemann-sum.md), and the elementary integral yields

$$
\begin{aligned}
\delta_N'(\theta)&\sim-\frac N\pi\int_0^\pi\frac{\sin a}{\cosh\theta+\cos a}da\\
&=-\frac N\pi\log\frac{\cosh\theta+1}{\cosh\theta-1}
=\frac{2N}{\pi}\log\tanh(\theta/2)
=\frac{16}{\gamma}\log\tanh(\theta/2).
\end{aligned}
$$

Since $\beta^2=8\pi/(N+1)$ and $\gamma=8\pi/N$, replacing $\gamma$ by $\beta^2$ changes this only at subleading order. The leading phase difference agrees with the standard semiclassical result. The derivative approximation is not uniform as $\theta\to0$ at fixed $N$; integrating its logarithm gives a finite leading phase difference nevertheless. A compatible constant is the given branch $\pi N$, whose choice is supplied by the exact amplitude rather than the classical trajectory.

As a useful endpoint check, $\int_0^\infty\log\tanh(u/2)du=-\pi^2/4$, obtained by expanding the two logarithms $\log(1-e^{-u})-\log(1+e^{-u})$. Thus the leading phase with coefficient $2N/\pi$ tends to $\pi N/2$. The exact unwrapped endpoints are

$$
\boxed{\delta_N(0)=\pi N,\qquad\delta_N(+\infty)=\frac{\pi(N+1)}2,}
$$

where the extra $\pi/2$ is subleading. Neither should be replaced by zero by an unannounced branch convention. Finally, the literal $m^2/\beta$ action gives a phase derivative of order $\sqrt N$, whereas the printed exact amplitude gives order $N$. **The requested exact/semiclassical matching requires correcting the overall action normalization to $m^2/\beta^2$.** This is an actual inconsistency between pages 2 and 4, not a change to the sine-Gordon equation or the classical scattering field.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 47](../../paper-47-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
