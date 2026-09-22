<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

A gauge symmetry is a local redundancy in the fields used to describe one physical state. With metric signature $(+---)$, define

$$
D_\mu=\partial_\mu+ieA_\mu,
\qquad
F_{\mu\nu}=\partial_\mu A_\nu-\partial_\nu A_\mu.
$$

The [quantum electrodynamics](../../../../../quantum-electrodynamics.md) Lagrangian is

$$
\mathcal L_{\mathrm{QED}}
=-\frac14F_{\mu\nu}F^{\mu\nu}
+\overline\psi(i\gamma^\mu D_\mu-m)\psi
=-\frac14F^2+\overline\psi(i\not\partial-m)\psi
-e\overline\psi\gamma^\mu\psi A_\mu.
$$

Under the local [U(1) gauge symmetry](../../../../../u-1-gauge-symmetry.md)

$$
\psi\mapsto e^{-ie\chi(x)}\psi,
\quad
\overline\psi\mapsto\overline\psi e^{ie\chi(x)},
\quad
A_\mu\mapsto A_\mu+\partial_\mu\chi,
$$

one has $D_\mu\psi\mapsto e^{-ie\chi}D_\mu\psi$ and $F_{\mu\nu}\mapsto F_{\mu\nu}$. Both terms in the Lagrangian are therefore invariant.

In [Feynman gauge](../../../../../feynman-gauge.md), the momentum-space [QED Feynman rules](../../../../../qed-feynman-rules.md) are:

- an internal electron line of momentum $r$: $i(\not r+m)/(r^2-m^2+i\epsilon)$;
- an internal photon line of momentum $k$: $-i\eta_{\mu\nu}/(k^2+i\epsilon)$;
- an electron-photon vertex: $-ie\gamma^\mu$, with four-momentum conserved;
- incoming and outgoing electrons: $u_s(p)$ and $\overline u_s(p)$;
- incoming and outgoing positrons: $\overline v_s(p)$ and $v_s(p)$ along the oriented fermion chain;
- incoming and outgoing photons: $\epsilon_\mu^{(\lambda)}(k)$ and $\epsilon_\mu^{(\lambda)*}(k)$.

One integrates each undetermined loop momentum, includes a factor $-1$ for each closed fermion loop, and imposes overall momentum conservation. None of the following tree diagrams contains a loop.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 301](../../paper-301-split.md)
3. [Iii](../../split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
