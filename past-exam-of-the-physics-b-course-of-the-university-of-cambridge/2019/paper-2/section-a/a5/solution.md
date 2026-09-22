<h1 id="section-a/a5/solution">Solution</h1>

↑ **Parent:** [A5](../a5.md)

For an ideal [electrical transformer](../../../../../transformer-electrical-engineering.md), let $n=N_p/N_s$. The reflected secondary load is $R_{\mathrm{in}}=n^2R_L$. Matching a $4\,\Omega$ load to an $8\,\Omega$ source therefore requires

$$
\boxed{n=\sqrt{\frac84}=\sqrt2.}
$$

With the generator replaced by its internal resistance, its resistance referred to the secondary is

$$
\boxed{R_{\mathrm{out}}=\left(\frac{N_s}{N_p}\right)^2(8\,\Omega)=4\,\Omega.}
$$

This is the source output resistance relevant to matching and maximum [power](../../../../../power.md) transfer.

To find the windings, use the [inductance of a toroidal winding](../../../../../inductance-of-a-toroidal-winding.md). The [mean](../../../../../expected-value-split.md) magnetic path is $\ell=2\pi(0.10)\,\mathrm m$, the core [area](../../../../../surface-area.md) is $A=30\times10^{-4}=0.003\,\mathrm{m^2}$ and $\mu=500\mu_0$. Thus

$$
L_p=\frac{\mu_0\mu_rN_p^2A}{\ell},
\qquad N_p=\sqrt{\frac{(0.75)2\pi(0.10)}{\mu_0(500)(0.003)}}=500.
$$

The ideal secondary turn count is $N_s=500/\sqrt2=353.55$, giving the practical nominal design

$$
\boxed{N_p=500,\qquad N_s\simeq354.}
$$

With integer turns the irrational ratio cannot be exact: $500:354$ reflects the $4\,\Omega$ load as $7.98\,\Omega$, an approximately $0.25\%$ resistance mismatch. These turn counts use the stated $0.75\,\mathrm H$ self-inductance; no operating [frequency](../../../../../frequency.md) was specified from which to set a separate minimum [inductance](../../../../../inductance.md).

The $200\,\Omega$ condition must refer to the unloaded magnetizing reactance, not to the matched loaded input resistance. With $L_p=0.75\,\mathrm H$,

$$
|X_p|=2\pi fL_p\geq200\,\Omega
\quad\Longrightarrow\quad f\geq42.4\,\mathrm{Hz}.
$$

The secondary self-inductance is $L_s=L_p/n^2=0.375\,\mathrm H$, so its corresponding unloaded coil impedance satisfies

$$
\boxed{Z_{s,\mathrm{coil}}=i\omega L_s,\qquad |Z_{s,\mathrm{coil}}|\geq100\,\Omega.}
$$

If output impedance means this transformed coil reactance, $100\,\Omega$ is its minimum magnitude. It is distinct from the $4\,\Omega$ transformed source resistance. This is the [magnetizing reactance and reflected resistance in a transformer](../../../../../magnetizing-reactance-and-reflected-resistance-in-a-transformer.md) distinction. A finite magnetizing [inductance](../../../../../inductance.md) adds a parallel branch, $Z_{\mathrm{in}}=(8\,\Omega)\parallel(i\omega L_p)$, so exact purely resistive matching is an ideal large-reactance approximation; interpreting the loaded input itself as both $8\,\Omega$ and at least $200\,\Omega$ would be impossible.

## ↑ Ancestors (14)

1. [A5](../a5.md)
2. [Section A](../../section-a.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2019](../../../split.md)
5. [Past exam of the physics B course of the University of Cambridge](../../../../split.md)
6. [Physics B course of the University of Cambridge](../../../../../physics-b-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
