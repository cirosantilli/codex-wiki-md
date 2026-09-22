<h1 id="19b/solution">Solution</h1>

↑ **Parent:** [19B](../19b.md)

Use the Maxwell curl equations

$$
\nabla\times\mathbf B=\mu_0\mathbf J+\mu_0\epsilon_0\mathbf E_t,\qquad
\nabla\times\mathbf E=-\mathbf B_t.
$$

Dot the first with $\mathbf E/\mu_0$ and the second with $\mathbf B/\mu_0$, then combine them. The identity $\nabla\cdot(\mathbf E\times\mathbf B)=\mathbf B\cdot\nabla\times\mathbf E-\mathbf E\cdot\nabla\times\mathbf B$ gives

$$
\partial_t\left(\frac{\epsilon_0}{2}E^2+\frac{B^2}{2\mu_0}\right)
=-\nabla\cdot\left(\frac{\mathbf E\times\mathbf B}{\mu_0}\right)-\mathbf J\cdot\mathbf E.
$$

This proves the [Poynting theorem](../../../../../poynting-theorem.md) **$W_t+\nabla\cdot\mathbf S+\mathbf J\cdot\mathbf E=0$**, with the stated energy density and [Poynting vector](../../../../../poynting-vector.md). The last term is work transferred from the electromagnetic field to matter.

For the specified vacuum wave, substitution into the same curl equations gives $kE_0=\omega B_0$ and $kB_0=\epsilon_0\mu_0\omega E_0$. Thus $\omega^2=k^2/\epsilon_0\mu_0$, and for propagation along positive $z$,

$$
\boxed{\omega=ck,\qquad c=(\epsilon_0\mu_0)^{-1/2},\qquad E_0=cB_0.}
$$

Putting $\vartheta=kz-\omega t$,

$$
\boxed{W=\epsilon_0E_0^2\cos^2\vartheta,\qquad
\mathbf S=\frac{E_0B_0}{\mu_0}\cos^2\vartheta\,\mathbf e_z=cW\mathbf e_z.}
$$

The equal electric and magnetic contributions account for the factor in $W$. Energy propagates at speed $c$, whose square is $1/(\epsilon_0\mu_0)$; the reciprocal product is not itself the speed.

## ↑ Ancestors (10)

1. [19B](../19b.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
