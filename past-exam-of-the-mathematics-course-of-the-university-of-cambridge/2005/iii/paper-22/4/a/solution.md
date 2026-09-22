<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Take a based [CW complex](../../../../../../cw-complex.md) model for $X$. Since it is $(n-1)$-connected and $n\ge2$, its reduced ordinary [homology](../../../../../../homology-split.md) vanishes below degree $n$, with arbitrary constant coefficients. This also follows from a [CW complex](../../../../../../cw-complex.md) model with no non-basepoint cells below degree $n$. The [connective spectrum](../../../../../../connective-spectrum.md) $E$ has $\pi_qE=0$ for $q<0$.

Filter $X$ by its skeleta. The quotients of consecutive stages are wedges of spheres, so the exact sequences in [represented homology theory](../../../../../../represented-homology-theory.md) give the [homological Atiyah-Hirzebruch spectral sequence](../../../../../../homological-atiyah-hirzebruch-spectral-sequence.md)

$$
E^2_{p,q}=\widetilde H_p(X;\pi_qE)\Longrightarrow\widetilde E_{p+q}(X),\qquad d_r:E^r_{p,q}\longrightarrow E^r_{p-r,q+r-1}.
$$

It is first quadrant because $E$ is a [connective spectrum](../../../../../../connective-spectrum.md). In a fixed total degree it converges with a finite filtration: cells of sufficiently high dimension cannot contribute in that degree or affect it through a boundary, by the same connectivity bound.

In total degree $n$, every term with $p<n$ is zero, and terms with $q<0$ are zero. The only possible term is

$$
E^2_{n,0}=\widetilde H_n(X;\pi_0E)=H_n(X;\mathbb Z).
$$

No differential can leave it: the target has spatial degree $n-r<n$. No differential can enter it: its source would be $(n+r,1-r)$, whose coefficient degree is negative for every $r\ge2$. Thus it survives unchanged and is the only filtration quotient of $\widetilde E_n(X)$; there is no extension problem. The ordinary [Hurewicz theorem](../../../../../../hurewicz-theorem.md) now yields

$$
\boxed{\widetilde E_n(X)\cong H_n(X;\mathbb Z)\cong\pi_n(X).}
$$

The isomorphism uses the stated identification $\pi_0E\cong\mathbb Z$ and is natural in $X$. This is the [bottom-degree generalized Hurewicz isomorphism](../../../../../../bottom-degree-generalized-hurewicz-isomorphism.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 22](../../../paper-22-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
