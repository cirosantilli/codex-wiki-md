<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Independence of the segment vectors makes the end-to-end distribution an $N$-fold [convolution](../../../../../convolution.md). Use the [characteristic function](../../../../../characteristic-function.md) convention $\widehat\psi(\mathbf k)=\int e^{i\mathbf k\cdot\mathbf r}\psi(\mathbf r)\,d^3r$. For a three-dimensional isotropic [freely jointed chain](../../../../../ideal-chain.md), the radial delta function fixes $|\mathbf r|=b$, and angular integration gives

$$
\widehat\psi(\mathbf k)=\frac1{4\pi}\int e^{ikb\cos\theta}\,d\Omega=\frac12\int_{-1}^1e^{ikb\mu}\,d\mu=\frac{\sin(kb)}{kb}.
$$

The [characteristic function of a sum of independent variables](../../../../../characteristic-function-of-a-sum-of-independent-variables.md) therefore gives $\widehat\Phi(\mathbf k,N)=[\sin(kb)/(kb)]^N$. In the central large-$N$ scaling, $k=O((b\sqrt N)^{-1})$, so

$$
N\ln\frac{\sin(kb)}{kb}=-\frac{Nb^2k^2}{6}+O(Nb^4k^4)=-\frac{Nb^2k^2}{6}+O(N^{-1}).
$$

Inverting this Gaussian [Fourier transform](../../../../../fourier-transform.md) yields

$$
\boxed{\Phi(\mathbf R,N)\sim\left(\frac3{2\pi Nb^2}\right)^{3/2}\exp\left[-\frac{3R^2}{2Nb^2}\right].}
$$

This [Gaussian limit of the end-to-end distribution of a freely jointed chain](../../../../../gaussian-limit-of-the-end-to-end-distribution-of-a-freely-jointed-chain.md) is normalized with respect to $d^3R$, has $\langle\mathbf R\rangle=0$ and $\langle R^2\rangle=Nb^2$, and is valid on the coil scale $R=O(b\sqrt N)$. If a density of the scalar distance $R$ is wanted instead, it is $4\pi R^2\Phi$. The Gaussian approximation does not describe the nearly fully stretched tail or the exact finite-chain cutoff at $R=Nb$.

For the scattering calculation, radial single-segment distributions together with the given independent-segment assumption imply rotational invariance of the whole chain. Therefore each pair separation $\mathbf S=\mathbf R_n-\mathbf R_m$ has a uniform direction conditional on its magnitude $S$. The same angular average gives

$$
\langle e^{i\mathbf k\cdot\mathbf S}\mid S\rangle=\frac12\int_{-1}^1e^{ikS\mu}\,d\mu=\frac{\sin(kS)}{kS}.
$$

Averaging its magnitude and then summing the pairs proves the required expression for the [polymer scattering function](../../../../../polymer-scattering-function.md):

$$
\boxed{g(k)=\frac1N\sum_{m,n=1}^N\left\langle\frac{\sin(k|\mathbf R_n-\mathbf R_m|)}{k|\mathbf R_n-\mathbf R_m|}\right\rangle.}
$$

The ratio has value one at zero separation, including every diagonal term $m=n$.

The printed gyration formula leaves $m$ unsummed. The intended [radius of gyration](../../../../../radius-of-gyration.md) must use a double pair sum, equivalently the mean square distance from the chain's [center of mass](../../../../../center-of-mass.md). To establish that equivalence, put $\mathbf R_{\rm cm}=N^{-1}\sum_n\mathbf R_n$ and expand both sides of

$$
\sum_{m,n}|\mathbf R_m-\mathbf R_n|^2=2N\sum_n|\mathbf R_n-\mathbf R_{\rm cm}|^2.
$$

Thus the consistent definition is $R_g^2=(2N^2)^{-1}\sum_{m,n}\langle|\mathbf R_m-\mathbf R_n|^2\rangle$. Expanding $\sin z/z=1-z^2/6+O(z^4)$ gives

$$
\begin{aligned}
g(k)&=N-\frac{k^2}{6N}\sum_{m,n}\langle|\mathbf R_m-\mathbf R_n|^2\rangle+O(k^4)\\
&=N\left[1-\frac{k^2R_g^2}{3}+O(k^4)\right].
\end{aligned}
$$

Therefore the general small-$k$ result is

$$
\boxed{\frac{g(k)}N=1-\frac{k^2R_g^2}{3}+O(k^4),\qquad kR_g\ll1.}
$$

This [Guinier expansion of a polymer scattering function](../../../../../guinier-expansion-of-a-polymer-scattering-function.md) requires isotropy and finite pair moments, but not [Gaussian distributions](../../../../../normal-distribution.md).

For a [Gaussian chain](../../../../../gaussian-chain.md), each pair difference across $\ell=|n-m|$ links has [variance](../../../../../variance-split.md) $\langle|\mathbf R_n-\mathbf R_m|^2\rangle=b^2\ell$ and [characteristic function](../../../../../characteristic-function.md) $e^{-k^2b^2\ell/6}$. Using exactly the $N$ scattering sites in the printed double sum, the finite-chain expression is

$$
\boxed{g_N(k)=1+\frac2N\sum_{\ell=1}^{N-1}(N-\ell)z^\ell=\frac{1+z}{1-z}-\frac{2z(1-z^N)}{N(1-z)^2},\qquad z=e^{-k^2b^2/6}.}
$$

The closed expression is understood by continuity at $z=1$, where it equals $N$. The factor $N-\ell$ counts pairs with $n=m+\ell$, with the prefactor two supplying their reversed order. In this finite-site convention,

$$
R_g^2=\frac{b^2}{N^2}\sum_{\ell=1}^{N-1}(N-\ell)\ell=\frac{b^2(N^2-1)}{6N}.
$$

This also holds for a [freely jointed chain](../../../../../ideal-chain.md) because its link covariances give the same mean square pair distances.

To obtain the complete long-chain scaling function, set $x=Nk^2b^2/6\simeq k^2R_g^2$ and replace contour sums by integrals, keeping $x$ fixed as $N\to\infty$. With $a=k^2b^2/6$,

$$
\begin{aligned}
g(k)&\sim\frac1N\int_0^N\int_0^Ne^{-a|n-m|}\,dn\,dm\\
&=\frac2N\int_0^N(N-s)e^{-as}\,ds
=\frac{2N(e^{-x}-1+x)}{x^2}.
\end{aligned}
$$

The requested [Debye scattering function for a Gaussian chain](../../../../../debye-scattering-function-for-a-gaussian-chain.md) is consequently

$$
\boxed{g(k)=N\mathcal D(k^2R_g^2),\qquad\mathcal D(x)=\frac{2(e^{-x}-1+x)}{x^2},\quad\mathcal D(0)=1,}
$$

exactly for the continuous Gaussian contour convention $R_g^2=Nb^2/6$, and asymptotically for the long discrete chain. Its small-$x$ expansion is $\mathcal D(x)=1-x/3+x^2/12+\cdots$, agreeing with the general gyration result, and $\mathcal D(x)\sim2/x$ at large $x$. In the continuum coil range $1\ll x\ll N$ this gives $g\sim12/(k^2b^2)$. At still larger $kb$, the discrete expression instead tends to the self-scattering value one.

There is a harmless finite-size convention in the source: $N$ links have $N+1$ endpoints, whereas its scattering sum counts $N$ sites. The formulas above retain its scattering normalization; if all endpoints are counted, replace the site count by $N+1$ in the finite formulas. The large-$N$ [Gaussian distribution](../../../../../normal-distribution.md) and Debye scaling function are unchanged to leading order.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 75](../../paper-75-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
