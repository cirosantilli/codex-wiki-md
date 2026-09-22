<h1 id="35d/solution">Solution</h1>

↑ **Parent:** [35D](../35d.md)

Ignoring magnetization, [electric polarization](../../../../../polarization-density.md) charge transport gives [bound current](../../../../../bound-current.md) $\mathbf J_{\rm b}=\partial_t\mathbf P$. The assumed weak dielectric contrast therefore gives $\mathbf J_{\rm b}\simeq-i\omega\epsilon_0(\epsilon_r-1)\mathbf E_0e^{i(\mathbf k\cdot\mathbf x-\omega t)}$ inside the [sphere](../../../../../sphere.md). This is the first [Born approximation](../../../../../born-approximation.md): the incident field supplies the [electric polarization](../../../../../polarization-density.md) to leading order in $\epsilon_r-1$.

For $\mathbf x=r\mathbf n$, the far-distance expansions are $|\mathbf x-\mathbf x'|=r-\mathbf n\cdot\mathbf x'+O(a^2/r)$ and $|\mathbf x-\mathbf x'|^{-1}\simeq r^{-1}$. Substitute the [retarded time](../../../../../retarded-time.md) into the phase in the [Lorenz gauge](../../../../../lorenz-gauge-condition.md) [vector potential](../../../../../vector-potential.md). The phase becomes $kr-\omega t+(\mathbf k-k\mathbf n)\cdot\mathbf x'$, so, using $\mu_0\epsilon_0=c^{-2}$,

$$
\boxed{\mathbf A_{\rm scatt}\simeq-\frac{i\omega(\epsilon_r-1)}{4\pi c^2r}\mathbf E_0e^{i(kr-\omega t)}I(q),\qquad
I(q)=\int_{|\mathbf x'|\leq a}e^{i\mathbf q\cdot\mathbf x'}d^3x',\quad\mathbf q=\mathbf k-k\mathbf n.}
$$

The assumptions $r\gg a$ and $ka^2/r\ll2\pi$ control amplitude and phase errors respectively. In the [radiation zone](../../../../../radiation-zone.md) the supplied electric and magnetic fields satisfy $\mathbf B_{\rm scatt}=c^{-1}\mathbf n\times\mathbf E_{\rm scatt}$. Complex phasors therefore give the time-averaged radial Poynting flux $|\mathbf E_{\rm scatt}|^2/(2\mu_0c)$. The incident flux is $|\mathbf E_0|^2/(2\mu_0c)$, so

$$
\frac{d\sigma}{d\Omega}=r^2\frac{|\mathbf E_{\rm scatt}|^2}{|\mathbf E_0|^2}
=\frac{(\epsilon_r-1)^2k^4}{16\pi^2}|I(q)|^2|\mathbf n\times\widehat{\mathbf E}_0|^2.
$$

Orient [spherical coordinates](../../../../../spherical-coordinate-system.md) along $\mathbf q$ to evaluate the form factor:

$$
I(q)=4\pi\int_0^a s^2\frac{\sin(qs)}{qs}\,ds=4\pi\frac{\sin(qa)-qa\cos(qa)}{q^3}.
$$

Consequently

$$
\boxed{\frac{d\sigma}{d\Omega}=(\epsilon_r-1)^2k^4\left[\frac{\sin(qa)-qa\cos(qa)}{q^3}\right]^2|\mathbf n\times\widehat{\mathbf E}_0|^2.}
$$

At $q=0$ the bracket is interpreted by its [limit](../../../../../limit-of-a-function.md) $a^3/3$, not a singularity. The transverse factor accounts for [polarization of an electromagnetic wave](../../../../../polarization-of-an-electromagnetic-wave.md); for complex [polarization of an electromagnetic wave](../../../../../polarization-of-an-electromagnetic-wave.md) its squared [norm](../../../../../norm.md) means the Hermitian [norm](../../../../../norm.md).

## ↑ Ancestors (10)

1. [35D](../35d.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
