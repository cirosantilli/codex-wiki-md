<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Take the [muon](../../../../../muon.md) [mass](../../../../../mass.md) to be $m_\mu$, and use the [quantum electrodynamics](../../../../../quantum-electrodynamics.md) convention $\mathcal L_{\rm int}=-e\bar\psi\gamma^\mu\psi A_\mu$ with $e>0$. Let $p_1,p_2$ be the incoming [muon](../../../../../muon.md) and antimuon momenta and $k_1,k_2$ the outgoing [photon](../../../../../photon.md) momenta, so $p_1+p_2=k_1+k_2$. External particles are [on shell](../../../../../on-shell.md): $p_1^2=p_2^2=m_\mu^2$ and $k_1^2=k_2^2=0$. The two tree-level [Feynman diagrams](../../../../../feynman-diagram.md) are the two orders in which the [photon](../../../../../photon.md) legs attach to the [muon](../../../../../muon.md) line. There is no three-[photon](../../../../../photon.md) [QED](../../../../../quantum-electrodynamics.md) vertex, and therefore no single-[photon](../../../../../photon.md) annihilation diagram into two [photons](../../../../../photon.md) at this order.

<a id="4/image-two-photon-orders-for-muon-annihilation-and-compton-scattering"></a>
![](../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-46-tree-diagrams.png)

**[Figure 1](#4/image-two-photon-orders-for-muon-annihilation-and-compton-scattering). Two photon orders for muon annihilation and Compton scattering**.

The [QED Feynman rules](../../../../../qed-feynman-rules.md) needed here are the vertex $-ie\gamma^\mu$, the [Dirac propagator](../../../../../dirac-propagator.md)

$$
\frac{i(\not q+m_\mu)}{q^2-m_\mu^2+i0},\qquad \not q=\gamma^\mu q_\mu,
$$

an incoming [muon](../../../../../muon.md) spinor $u(p_1)$, an incoming antimuon adjoint $\bar v(p_2)$, and an outgoing [photon](../../../../../photon.md) polarization $\epsilon_\mu^*(k)$. At a vertex enforce [four-momentum](../../../../../four-momentum.md) conservation. Spinor products are ordered along the [fermion](../../../../../fermion.md) line; exchanging the external [photons](../../../../../photon.md) introduces no relative minus sign. Define $R(q)=(\not q+m_\mu)/(q^2-m_\mu^2+i0)$ and $\not\epsilon=\gamma^\mu\epsilon_\mu$.

With the convention that a diagram contributes $i\mathcal M$, the two [muon](../../../../../muon.md)-antimuon annihilation amplitudes are

$$
\begin{aligned}
\mathcal M_t&=-e^2\bar v(p_2)\not\epsilon_2^*R(p_1-k_1)\not\epsilon_1^*u(p_1),\\
\mathcal M_u&=-e^2\bar v(p_2)\not\epsilon_1^*R(p_1-k_2)\not\epsilon_2^*u(p_1),\\
\boxed{\mathcal M_{\rm ann}}&\boxed{=\mathcal M_t+\mathcal M_u.}
\end{aligned}
$$

Their denominators are respectively $t-m_\mu^2+i0$ and $u-m_\mu^2+i0$, where $t=(p_1-k_1)^2$, $u=(p_1-k_2)^2$. A different consistent overall amplitude-phase convention has no physical effect.

A physical [photon polarization vector](../../../../../photon-polarization-vector.md) obeys **$k\cdot\epsilon=0$**, and represents an equivalence class $\epsilon\sim\epsilon+\alpha k$. For a real null momentum, adding $\alpha k$ preserves transversality. One can additionally choose transverse spatial vectors with $\epsilon^0=0$ and $\epsilon^*\cdot\epsilon=-1$; there are two independent physical polarizations. The equivalence class removes the unphysical longitudinal direction, rather than imposing four independent physical polarization states.

The invariance of the total amplitude is a [two-photon fermion Ward identity](../../../../../two-photon-fermion-ward-identity.md). Replace $\epsilon_1^*$ by $k_1$ and put $q_t=p_1-k_1$, $q_u=p_1-k_2=k_1-p_2$. The external [Dirac equations](../../../../../dirac-equation.md) give

$$
(\not p_1-m_\mu)u(p_1)=0,\qquad \bar v(p_2)(\not p_2+m_\mu)=0.
$$

Away from propagator poles, $R(q)(\not q-m_\mu)=(\not q-m_\mu)R(q)=I$; the identity extends with the common Feynman prescription. Therefore

$$
\begin{aligned}
R(q_t)\not k_1u(p_1)&=R(q_t)(\not p_1-\not q_t)u(p_1)=-u(p_1),\\
\bar v(p_2)\not k_1R(q_u)&=\bar v(p_2)(\not q_u+\not p_2)R(q_u)=\bar v(p_2).
\end{aligned}
$$

The two terms in the bracket then give $-\bar v\not\epsilon_2^*u$ and $+\bar v\not\epsilon_2^*u$, which cancel. Exchanging [photon](../../../../../photon.md) labels proves the second [Ward identity](../../../../../ward-identity.md). Thus **the sum is unchanged under $\epsilon_i\mapsto\epsilon_i+\alpha k_i$ for either [photon](../../../../../photon.md)**. Neither diagram is generally [gauge-invariant](../../../../../gauge-invariance.md) separately. Physically, longitudinal pure-gauge polarization does not couple to the observable [scattering amplitude](../../../../../scattering-amplitude.md); only the two transverse [photon](../../../../../photon.md) degrees of freedom contribute.

For [Compton scattering](../../../../../compton-scattering.md) write the incoming momenta as $p,k$ and outgoing momenta as $p',k'$, with $p+k=p'+k'$. The outgoing [muon](../../../../../muon.md) contributes $\bar u(p')$, the incoming [photon](../../../../../photon.md) contributes $\epsilon(k)$ without conjugation, and the outgoing [photon](../../../../../photon.md) contributes $\epsilon'^*(k')$. The two [tree-level Compton amplitudes](../../../../../tree-level-compton-amplitude.md) are

$$
\begin{aligned}
\mathcal M_s&=-e^2\bar u(p')\not\epsilon'^*R(p+k)\not\epsilon\,u(p),\\
\mathcal M_u&=-e^2\bar u(p')\not\epsilon\,R(p-k')\not\epsilon'^*u(p),\\
\boxed{\mathcal M_{\rm C}}&\boxed{=\mathcal M_s+\mathcal M_u.}
\end{aligned}
$$

These are the lower two diagrams. Their intermediate [muon](../../../../../muon.md) momenta are $p+k$ and $p-k'$, with denominators $s-m_\mu^2+i0$ and $u-m_\mu^2+i0$. The first attaches the incoming [photon](../../../../../photon.md) before the outgoing [photon](../../../../../photon.md) along [fermion](../../../../../fermion.md) flow; the second reverses that attachment order. Both contribute at order $e^2$ in the amplitude.

**[Compton scattering](../../../../../compton-scattering.md) has one incoming and one outgoing [muon](../../../../../muon.md) and one [photon](../../../../../photon.md) on each side; annihilation has an incoming particle-[antiparticle](../../../../../antiparticle.md) pair and two outgoing [photons](../../../../../photon.md).** Accordingly the external spinors/polarizations and physical Mandelstam channels differ, although both arise from the same two-vertex [QED](../../../../../quantum-electrodynamics.md) matrix element. [Crossing symmetry](../../../../../crossing-symmetry.md) relates them by continuing $p_2\mapsto-p'$ and one outgoing [photon](../../../../../photon.md) momentum $k_1\mapsto-k$, with the corresponding external wavefunction replacements. The annihilation $t$ channel becomes the Compton $s$ channel and the other channel becomes its $u$ channel. Identical final [photons](../../../../../photon.md) require a factor $1/2!$ in an annihilation phase-space integral over an otherwise double-counted full final-state region; there is no analogous final-state identical-particle factor for the [muon](../../../../../muon.md)-[photon](../../../../../photon.md) Compton final state. Gauge cancellation holds for the summed Compton amplitude as well.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 46](../../paper-46-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
