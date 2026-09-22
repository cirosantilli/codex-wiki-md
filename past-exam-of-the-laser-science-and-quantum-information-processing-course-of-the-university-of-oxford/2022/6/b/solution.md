<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Starting at port 1, the first [beam splitter](../../../../beam-splitter.md) encounter sends amplitude $c$ straight out through port 0 and stores amplitude $-c$ towards M2. A return from M2 enters port $1'$; it sends the stored amplitude times $-c$ out through port 1 and times $c$ towards M1. A return from M1 enters port $0'$; it sends amplitude times $c$ out through port 0 and times $c$ towards M2. Both internal continuations carry $+c$, so two additional encounters multiply the surviving amplitude by $+c^2$.

With the fixed mirror and propagation phases absorbed as in [a](../a.md), the nonzero coefficients of the outgoing [single-photon state](../../../../single-photon-state.md) are

$$
\boxed{\begin{aligned}
c_{0,1}&=2^{-1/2},\\
c_{0,2j+1}&=-2^{-(2j+1)/2},&&j=1,2,3,\ldots,\\
c_{1,2j}&=2^{-j},&&j=1,2,3,\ldots,
\end{aligned}}
$$

and $c_{0,2j}=c_{1,2j+1}=0$. The first nonzero terms are $c_{0,1}=1/\sqrt2$, $c_{1,2}=1/2$, $c_{0,3}=-1/(2\sqrt2)$ and $c_{1,4}=1/4$. If fixed reflection amplitudes $r_1,r_2$ are retained instead, multiply $c_{0,2j+1}$ by $(r_1r_2)^j$ and $c_{1,2j}$ by $r_2^jr_1^{j-1}$, as well as the appropriate delay propagation phases. These unit-modulus factors do not alter the following probabilities.

Distinct exit events are orthogonal because they differ in output port or arrival-time bin. This requires the incident wavepacket to resolve the delay. Summing the squared moduli as [geometric series](../../../../geometric-series.md) gives

$$
\boxed{P(0)=\sum_{j=0}^\infty2^{-(2j+1)}=\frac23,\qquad
P(1)=\sum_{j=1}^\infty2^{-2j}=\frac13.}
$$

Their sum is one. After $n$ encounters the probability of still being inside is $2^{-n}$, which tends to zero, so no trapped component is omitted.

The source drawing places the delay line in the M2 arm. A visit to M2 crosses that line in both directions. If $\tau$ is its **one-way** delay, then an exit after $n$ encounters has crossed it $2\lfloor n/2\rfloor$ times:

$$
\boxed{t_n=2\tau\lfloor n/2\rfloor
=\begin{cases}(n-1)\tau,&n\ \text{odd},\\n\tau,&n\ \text{even}.\end{cases}}
$$

If the phrase “delay time $\tau$” instead denotes the complete M2-arm round-trip delay, replace $2\tau$ by $\tau$ in the floor formula. The wording does not explicitly distinguish these conventions. Consecutive encounters can produce the same exit time in different ports: for example $n=2,3$ both follow one M2 visit. If the incident wavepacket were much longer than the arm delay, different histories in the same port would overlap and their [probability amplitudes](../../../../probability-amplitude.md) would have to be added before squaring; the asserted time-bin expansion would then not be an orthonormal event basis.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [6](../../6.md)
3. [2022](../../../2022-split.md)
4. [Past exam of the laser science and quantum information processing course of the University of Oxford](../../../split.md)
5. [Laser science and quantum information processing course of the University of Oxford](../../../../laser-science-and-quantum-information-processing-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
