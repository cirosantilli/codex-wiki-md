<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Take incoming electron momentum $p$ and positron momentum $q$, with outgoing photon momenta $k_1,k_2$, so $p+q=k_1+k_2$. The leading [electron-positron annihilation into two photons](../../../../../electron-positron-annihilation-into-two-photons.md) has two [tree-level Feynman diagrams](../../../../../tree-level-feynman-diagram.md), differing by the order in which the two outgoing photons attach to the charged-fermion line.

<a id="4/image-the-two-photon-orders-in-electron-positron-annihilation-and-the-s-and-u-channels-of-compton-scattering"></a>
![](../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-44-two-photon-diagrams.png)

**[Figure 1](#4/image-the-two-photon-orders-in-electron-positron-annihilation-and-the-s-and-u-channels-of-compton-scattering). The two photon orders in electron-positron annihilation and the s and u channels of Compton scattering**.

The arrows indicate [fermion flow](../../../../../fermion-flow.md). An incoming positron has the opposite flow direction to its physical momentum; the lower row uses an outgoing electron instead.

The required [QED Feynman rules](../../../../../qed-feynman-rules.md), with interaction $-e\bar\psi\gamma^\mu\psi A_\mu$, are a vertex $-ie\gamma^\mu$, a [Dirac propagator](../../../../../dirac-propagator.md) $i(\not r+m)/(r^2-m^2+i0)$, an incoming electron spinor $u(p)$, an incoming positron adjoint $\bar v(q)$, and an outgoing photon polarization $\epsilon^*_\mu(k)$. Here [Feynman slash notation](../../../../../feynman-slash-notation.md) means $\not a=\gamma^\mu a_\mu$, and the external [Dirac equations](../../../../../dirac-equation.md) are $(\not p-m)u(p)=0$ and $\bar v(q)(\not q+m)=0$.

Put $\mathcal S(r)=(\not r+m)/(r^2-m^2+i0)$, omitting only the propagator's overall factor $i$. Multiplying the two vertices and the propagator gives

$$
\boxed{\mathcal M=-e^2\bar v(q)\left[
\not\epsilon_2^*\mathcal S(p-k_1)\not\epsilon_1^*
+\not\epsilon_1^*\mathcal S(p-k_2)\not\epsilon_2^*
\right]u(p).}
$$

The diagrammatic expression is $i\mathcal M$. The relative sign is plus because the two photons are bosons; exchanging their attachments does not exchange external fermions. The amplitude is of order $e^2$.

A physical [photon polarization vector](../../../../../photon-polarization-vector.md) obeys $k^2=0$ and $k\cdot\epsilon=0$, with the gauge equivalence $\epsilon\sim\epsilon+\alpha k$. One can choose a transverse representative with $\epsilon^0=0$ and normalize $\epsilon^*\cdot\epsilon=-1$. There are two physical transverse polarizations.

To prove the requested [two-photon fermion Ward identity](../../../../../two-photon-fermion-ward-identity.md), replace $\epsilon_1^*$ by $k_1$. Away from an internal pole, $\mathcal S(r)$ is the inverse of $\not r-m$, with the boundary prescription understood. The first term simplifies because

$$
\not k_1=(\not p-m)-(\not p-\not k_1-m),\qquad
\mathcal S(p-k_1)\not k_1u(p)=-u(p).
$$

For the second term, [four-momentum conservation](../../../../../four-momentum-conservation.md) gives $k_1=(p-k_2)+q$, so

$$
\bar v(q)\not k_1\mathcal S(p-k_2)
=\bar v(q)[(\not p-\not k_2-m)+(\not q+m)]\mathcal S(p-k_2)
=\bar v(q).
$$

The two contributions are therefore $-\bar v\not\epsilon_2^*u$ and $+\bar v\not\epsilon_2^*u$, which cancel. Interchanging the photon labels proves the other contraction vanishes. By linearity, **adding a multiple of either photon momentum to its polarization leaves the summed amplitude unchanged**. This is [gauge invariance](../../../../../gauge-invariance.md): longitudinal gauge representatives do not describe an additional physical photon state. An individual diagram does not generally have this property.

For [Compton scattering](../../../../../compton-scattering.md), let $p,k$ be incoming electron and photon momenta and $p',k'$ the outgoing ones. The diagrams in the lower row have intermediate electron momenta $p+k$ and $p-k'$ respectively. The same [QED Feynman rules](../../../../../qed-feynman-rules.md) give

$$
\boxed{\mathcal M_C=-e^2\bar u(p')\left[
\not\epsilon'^*\mathcal S(p+k)\not\epsilon
+\not\epsilon\mathcal S(p-k')\not\epsilon'^*
\right]u(p).}
$$

Their denominators are $(p+k)^2-m^2+i0$ and $(p-k')^2-m^2+i0$, the $s$- and $u$-channel denominators. In annihilation the two exchanged-electron channels instead carry $p-k_1$ and $p-k_2$. [Crossing symmetry](../../../../../crossing-symmetry.md) relates the two expressions by moving the positron to an outgoing electron and one outgoing photon to an incoming photon, with the corresponding momentum and polarization replacements. There is no two-photon contact vertex for the minimally coupled Dirac electron. Both processes require the sum of the two photon orders to satisfy the [Ward identity](../../../../../ward-identity.md).

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 44](../../paper-44-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
