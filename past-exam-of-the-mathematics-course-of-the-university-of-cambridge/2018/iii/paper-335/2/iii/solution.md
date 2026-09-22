<h1 id="2/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Let $H$ be the measured [wave scattering](../../../../../../wave-scattering.md) response\> [linear operator](../../../../../../linear-operator.md), with direct background propagation removed if present. Its [time reversal operator](../../../../../../time-reversal-operator.md) is the [positive operator](../../../../../../positive-operator.md) $T=H^*H$. For a normalized emitted signal $h$,

$$
\|Hh\|^2=\langle Th,h\rangle,\qquad
\max_{\|h\|=1}\|Hh\|^2=\lambda_{\max}(T)=\sigma_{\max}(H)^2.
$$

The maximizing signal is a right [singular vector](../../../../../../singular-vector.md), equivalently an [eigenvector](../../../../../../eigenvector.md) of $T$ with its largest [eigenvalue](../../../../../../eigenvalue.md). This is a precise intensity statement independent of a scatterer model.

Under the [Born approximation for scalar wave scattering](../../../../../../born-approximation-for-scalar-wave-scattering.md), neglect interactions between [point scatterers](../../../../../../point-scatterer.md) and write

$$
H\simeq\sum_j\alpha_jb_jc_j^*,
$$

where $b_j$ is the receiver response to scatterer $j$, $c_j^*h$ is its illumination by the source array, and $\alpha_j$ is its scattering [wave amplitude](../../../../../../wave-amplitude.md). Well-resolved [point scatterers](../../../../../../point-scatterer.md) have approximately [orthogonal vectors](../../../../../../orthogonal-vectors.md) $b_j$ and $c_j$. In the ideal [orthogonal](../../../../../../orthogonal-vectors.md) limit,

$$
H^*H=\sum_j|\alpha_j|^2\|b_j\|^2c_jc_j^*,\qquad
\boxed{\lambda_j=|\alpha_j|^2\|b_j\|^2\|c_j\|^2.}
$$

Thus the most reflective, geometrically weighted scatterer gives the largest [eigenvalue](../../../../../../eigenvalue.md), and its normalized steering vector $c_j/\|c_j\|$ gives the corresponding [wave focusing](../../../../../../wave-focusing.md) signal. If illumination and reception factors are equal for all scatterers, this is precisely the scatterer with largest $|\alpha_j|^2$. Geometric size by itself is not the quantity being ranked.

Repeated adjoint [time reversal acoustics](../../../../../../time-reversal-acoustics.md) is [power iteration](../../../../../../power-iteration.md) on $T$. If its top [eigenvalue](../../../../../../eigenvalue.md) is simple and the initial signal has a nonzero component along its [eigenvector](../../../../../../eigenvector.md), then

$$
\frac{T^nh}{\|T^nh\|}\longrightarrow e^{i\theta}v_{\max}.
$$

A tied largest [eigenvalue](../../../../../../eigenvalue.md) leaves a combination in the leading [eigenspace](../../../../../../eigenspace.md), and an initial signal [orthogonal](../../../../../../orthogonal-vectors.md) to that [eigenspace](../../../../../../eigenspace.md) cannot excite it. This is the basis of the [DORT method](../../../../../../dort-method.md). Mere physical separation is insufficient if the array cannot resolve the scatterers; coherent steering-vector overlap or [multiple scattering](../../../../../../multiple-scattering.md) can mix the modes. Also, if $H$ includes unrestricted homogeneous transmission, its largest [eigenvalue](../../../../../../eigenvalue.md) need not identify any individual scatterer. The correspondence concerns the resolved [wave scattering](../../../../../../wave-scattering.md) response\>. The ideal correspondence and selective [wave focusing](../../../../../../wave-focusing.md) are analyzed by [Prada and Fink](https://www.institut-langevin.espci.fr/IMG/pdf/PradaFink_WaveMotion_1994.pdf).

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [2](../../2.md)
3. [Paper 335](../../../paper-335-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
