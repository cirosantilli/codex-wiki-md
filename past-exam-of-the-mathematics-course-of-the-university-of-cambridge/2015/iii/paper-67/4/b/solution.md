<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the [Fourier transform](../../../../../../fourier-transform.md) convention $\widehat w(E)=\int_{\mathbb R}w(t)e^{itE}\,dt$ and define the [spectral filtering of Hamiltonian terms](../../../../../../spectral-filtering-of-hamiltonian-terms.md) by

$$
\boxed{g^{(Z)}=\int_{\mathbb R}
w(t)e^{itH}h_Ze^{-itH}\,dt.}
$$

The normalization $\widehat w(0)=1$ means $\int w=1$. Since $w$ is real and nonnegative, $\widehat w(-E)=\overline{\widehat w(E)}$. Thus the stated positive-frequency cutoff also implies $\widehat w(E)=0$ for $E\leq-\Delta$. The integral exists in [operator norm](../../../../../../operator-norm.md), because its integrand has norm at most $w(t)\|h_Z\|$.

Let $H|\phi_i\rangle=E_i|\phi_i\rangle$, with $E_i-E_0\geq\Delta$ for $i>0$. In this [eigenbasis](../../../../../../eigenbasis.md),

$$
\langle\phi_i|g^{(Z)}|\phi_j\rangle
=\widehat w(E_i-E_j)\langle\phi_i|h_Z|\phi_j\rangle.
$$

Every matrix element coupling the unique [ground state](../../../../../../ground-state.md) to an excited state vanishes, in either direction. Hence

$$
\boxed{[g^{(Z)},P_0]=0,\qquad
g^{(Z)}|\phi_0\rangle
=\langle\phi_0|h_Z|\phi_0\rangle|\phi_0\rangle.}
$$

Moreover, linearity and conservation of $H$ under its own [Heisenberg picture](../../../../../../heisenberg-picture.md) evolution give

$$
\sum_Zg^{(Z)}
=\int w(t)e^{itH}\left(\sum_Zh_Z\right)e^{-itH}\,dt
=H\int w(t)\,dt
=\boxed{H.}
$$

Each filtered term is Hermitian, but it need not remain supported on its original set $Z$. The tail assumption supplies stronger long-time control than the integrability used here; no additional tail estimate is needed for the requested identities.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 67](../../../paper-67-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
