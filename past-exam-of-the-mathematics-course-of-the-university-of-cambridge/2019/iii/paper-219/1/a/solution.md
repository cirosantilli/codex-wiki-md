<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let

$$
C_k=\sigma_{\mathrm{int}}^2+\sigma_{m,k}^2+\sigma_{C,k}^2,
\qquad
H_i=\sigma_{\mathrm{int}}^2+\sigma_{m,i}^2.
$$

Subtracting the measured [distance modulus](../../../../../../distance-modulus.md) from the measured [apparent magnitude](../../../../../../apparent-magnitude.md) gives

$$
q_k=\widehat m_k-\widehat\mu_{C,k}\sim N(M_0,C_k).
$$

For the [Hubble flow](../../../../../../hubble-flow.md), define

$$
r_i=\widehat m_i-25-5\log_{10}\!\left(\frac{cz_i}{100\ {\rm km\,s^{-1}}}\right).
$$

The [Hubble law](../../../../../../hubble-s-law.md), with the [Hubble constant](../../../../../../hubble-constant.md) parametrized by $\theta=5\log_{10}h$, gives $r_i\sim N(M_0-\theta,H_i)$. After integrating over each intrinsic [absolute magnitude](../../../../../../absolute-magnitude.md) and each unobserved true distance modulus, independence therefore gives the [likelihood function](../../../../../../likelihood-function.md)

$$
\boxed{
L(M_0,\theta)=
\prod_{k=1}^K\frac{e^{-(q_k-M_0)^2/(2C_k)}}{\sqrt{2\pi C_k}}
\prod_{i=1}^N\frac{e^{-(r_i-M_0+\theta)^2/(2H_i)}}{\sqrt{2\pi H_i}}.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 219](../../../paper-219-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
