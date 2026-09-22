<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The sign of cluster evolution depends on the orbital energy of the captured stars, not just on their small angular momentum. Let the instantaneous capture rate be $\Gamma>0$, so the remaining stellar mass $M_s=Nm$ has $\dot M_s=-m\Gamma$, while $\dot M_H\simeq m\Gamma$. A captured star has negative specific orbital energy $\epsilon_{\rm cap}$ measured outside the absorbing region. Removing it increases the energy of the surviving stars by $-m\epsilon_{\rm cap}$; growth of the central [black hole](../../../../../../black-hole.md) instead deepens their potential.

To turn this balance into a radius estimate, assume the surviving cluster evolves slowly through homologous virial equilibria of scale $R$. Write its stellar self-energy and black-hole interaction energy as

$$
W_{ss}=-a\frac{GM_s^2}R,\qquad
U_H=-b\frac{GM_HM_s}R,
$$

where positive $a,b$ depend on the density shape. The [virial theorem](../../../../../../virial-theorem.md) gives

$$
E=\frac{W_{ss}+U_H}{2}
=-\frac G{2R}\mathcal P,
\qquad\mathcal P=aM_s^2+bM_HM_s.
$$

At the instant of capture, the stellar-system energy budget, excluding feedback and energy carried by other escaping stars, is

$$
\dot E=-m\Gamma\epsilon_{\rm cap}
-G\dot M_H\int\frac{dM_s}{r}
=-m\Gamma\epsilon_{\rm cap}-\frac{bGM_s\dot M_H}R.
$$

The second term is the work of the changing central potential; it must not be confused with the change in the number of stars. Differentiating the virial expression and using $\dot M_H=m\Gamma$ gives

$$
\boxed{\frac{\dot R}R=
\frac{m\Gamma}{aM_s^2+bM_HM_s}
\left[-\frac{2R\epsilon_{\rm cap}}G-(2a+b)M_s-bM_H\right].}
$$

This estimates the radius response of a general homologous cluster once its structure and capture energies are specified.

For a simpler locally Keplerian subsystem, neglect its stellar self-gravity, so $E=-bGM_HM_s/(2R)$. Put $\epsilon_{\rm cap}=\xi E/M_s$, with $\xi>0$ measuring how tightly bound a captured star is relative to the average orbital energy. The preceding balance reduces to

$$
\boxed{\frac{\dot R}R\simeq(\xi-1)\frac\Gamma N-\frac{m\Gamma}{M_H}.}
$$

This is [Keplerian cluster radius evolution under stellar capture](../../../../../../keplerian-cluster-radius-evolution-under-stellar-capture.md). Removing representative-energy stars, $\xi=1$, leaves unchanged the characteristic orbits if $M_H$ is fixed; with black-hole growth it contracts them at rate $\dot R/R\simeq-\dot M_H/M_H$. Preferential removal of more tightly bound stars drives expansion if $\xi-1>M_s/M_H$. In that heating-dominated case,

$$
t_R\equiv\left|\frac{\dot R}R\right|^{-1}
\sim\frac{N}{|\xi-1|\Gamma},
$$

so inserting the empty-cone flux gives $t_R\sim t_{\rm rel}\log(1/\mathcal R_{\rm lc})/|\xi-1|$ for the one-zone estimate. Growth-dominated contraction instead has timescale $M_H/(m\Gamma)$.

For a Kepler orbit of semimajor axis $a_{\rm cap}$, $\epsilon_{\rm cap}=-GM_H/(2a_{\rm cap})$ and $\xi=R/(ba_{\rm cap})$. Reaching $R_{\rm sch}$ does not imply that the orbit had binding energy of order $c^2$: a nearly parabolic star can reach that pericentre with almost zero orbital energy. **Therefore expansion is expected when strongly bound central stars are preferentially swallowed, but the supplied information does not uniquely fix the sign or rate for the entire remaining cluster.** Captured-energy selection, the density profile and any energy feedback must be specified. The balances above give both the conventional expansion estimate and the contraction case without assuming missing data.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 44](../../../paper-44-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
