<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

**Gibbs free energy and its minimum.** For fixed atom number $N$, there are $N+n$ sites and

$$
W(N,n)=\binom{N+n}{n}
$$

configurations with $n$ indistinguishable vacancies. Their [configurational entropy](../../../../configurational-entropy.md) is $k_B\ln W$. Relative to the vacancy-free [Gibbs free energy](../../../../gibbs-free-energy.md) $G_0$, creating $n$ vacancies costs [energy](../../../../energy-split.md) $n\epsilon$ and pressure-[volume](../../../../volume.md) work $npv$. Put $A=\epsilon+pv>0$. Then

$$
G(n)=G_0+nA-k_BT\ln\frac{(N+n)!}{N!\,n!}.
$$

At leading thermodynamic order, [Stirling's approximation](../../../../stirling-formula.md) gives

$$
G(n)\simeq G_0+nA-k_BT\big[(N+n)\ln(N+n)-N\ln N-n\ln n\big].
$$

The minimum obtained from the stationary point below is

$$
\boxed{G_{\min}\simeq G_0+Nk_BT\ln\left(1-e^{-A/(k_BT)}\right).}
$$

If the perfect crystal's [internal energy](../../../../internal-energy-split.md) and other [entropy](../../../../entropy-split.md) are chosen as zero, its [pressure](../../../../pressure-split.md) term is $G_0=pNv$. More generally the information given fixes the vacancy contribution rather than the absolute bulk [free energy](../../../../thermodynamic-free-energy.md). The pressure-[volume](../../../../volume.md) term must be retained because the number of sites, and hence the [volume](../../../../volume.md), changes.

**Equilibrium vacancy population.** Differentiating the extensive [free energy](../../../../thermodynamic-free-energy.md) at fixed $N,T,p$ gives

$$
\frac{\partial G}{\partial n}=A+k_BT\ln\frac n{N+n},\qquad
\frac{\partial^2G}{\partial n^2}=\frac{k_BTN}{n(N+n)}>0.
$$

The stationary point is consequently the unique interior minimum. Write $q=e^{-A/(k_BT)}$; its condition is $n/(N+n)=q$, giving the requested thermodynamic result for [equilibrium vacancies with variable lattice size](../../../../equilibrium-vacancies-with-variable-lattice-size.md),

$$
\boxed{n_*\simeq\frac{Nq}{1-q}
=\frac{N}{e^{(\epsilon+pv)/(k_BT)}-1}.}
$$

Substitution back into $G$ cancels the terms containing $n_*$ and yields the boxed minimum. In the dilute-defect limit $A\gg k_BT$, $n_*\simeq Ne^{-A/(k_BT)}$. The Bose-like denominator is a consequence of the changing number of lattice sites and combinatorial [entropy](../../../../entropy-split.md); it does not assert that vacancies here are an ideal gas of bosonic particles.

There is a [finite-size correction to a variable-site vacancy model](../../../../finite-size-correction-to-a-variable-site-vacancy-model.md) if “average” is interpreted exactly. The microscopic count written above gives the relative isothermal-isobaric sum

$$
\mathcal Y=\sum_{n=0}^\infty\binom{N+n}{n}q^n=(1-q)^{-N-1},
$$

so

$$
\boxed{\langle n\rangle_{\rm exact}=q\partial_q\ln\mathcal Y
=\frac{(N+1)q}{1-q}.}
$$

Its relative equilibrium [free energy](../../../../thermodynamic-free-energy.md) is $-k_BT\ln\mathcal Y=(N+1)k_BT\ln(1-q)$. Thus the source's $N$ numerator is correct to leading extensive order, but is not the exact finite-$N$ mean for that stated configuration count. A free-[energy](../../../../energy-split.md) minimum is likewise not generally identical to the mean of a finite distribution. These distinctions vanish relatively as $N\to\infty$.

**Thermal volume.** Each atom or vacancy occupies [volume](../../../../volume.md) $v$, so at the same thermodynamic accuracy

$$
\boxed{\langle V(T)\rangle\simeq v(N+n_*)
=\frac{Nv}{1-e^{-(\epsilon+pv)/(k_BT)}}.}
$$

For the exact counting model, replace $n_*$ by $(N+1)q/(1-q)$ in $v(N+\langle n\rangle)$. The vacancy-free limit is $Nv$ as $T\to0$. This model isolates expansion from vacancies, taking $v$ and $\epsilon$ constant; it omits ordinary [phonon](../../../../phonon.md) thermal expansion. Its growth at high [temperature](../../../../temperature-split.md) should not be extrapolated to arbitrarily large vacancy fractions in a stable crystal, and $A>0$ is essential for a normalizable variable-site ensemble.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [3](../../3.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the thermal and statistical physics course of the University of Cambridge](../../../split.md)
5. [Thermal and Statistical Physics course of the University of Cambridge](../../../../thermal-and-statistical-physics-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)
