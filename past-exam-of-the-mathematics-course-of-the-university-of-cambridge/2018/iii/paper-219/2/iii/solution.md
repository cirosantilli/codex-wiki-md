<h1 id="2/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Choose a fixed $H_{\rm ref}>0$, and write $h(H_0)=-5\log_{10}(H_0/H_{\rm ref})$ and $d_s(w,\Omega_M)=\mu(z_s;H_{\rm ref},w,\Omega_M)$. The predicted magnitude is $M_0+h(H_0)+d_s$. Thus the likelihood depends on $M_0,H_0$ only through $\beta=M_0+h(H_0)$, the [absolute magnitude–Hubble constant degeneracy](../../../../../../absolute-magnitude-hubble-constant-degeneracy.md). Since $dM_0=d\beta$ at fixed $H_0$, integrating with a flat density over the entire real line removes $H_0$.

Explicitly, let $a_s=(v+r_s)^{-1}$, $S=\sum_sa_s$, $x_s=\widehat m_s-d_s$, $\bar x=S^{-1}\sum_sa_sx_s$ and $Q=\sum_sa_s(x_s-\bar x)^2$. Completing the square gives $\sum_sa_s(x_s-\beta)^2=Q+S(\beta-\bar x)^2$, so [flat-prior elimination of a Gaussian common mean](../../../../../../flat-prior-elimination-of-a-gaussian-common-mean.md) yields

$$
\boxed{I\propto(2\pi)^{-(N-1)/2}S^{-1/2}\prod_s(v+r_s)^{-1/2}e^{-Q/2}},
$$

independently of $H_0$. The proportionality includes the arbitrary constant of the flat prior, which cancels within this posterior analysis.

If the remaining posterior integral is finite, prior independence gives $p(H_0\mid\mathcal D)\propto p(H_0)$ and hence $\boxed{p(H_0\mid\mathcal D)=p(H_0)}$: these data supply no marginal update of the [Hubble constant](../../../../../../hubble-constant.md). The quoted Gaussian is consequently retained with its stated $a,b$. Strictly, the model uses $H_0>0$ inside a logarithm, so the Gaussian prior must be restricted and normalized on that domain:

$$
p(H_0\mid\mathcal D)=\frac{\phi((H_0-a)/b)}{b\Phi(a/b)}\mathbf1_{\{H_0>0\}},
$$

where $\phi,\Phi$ are the standard normal density and distribution function. Ignoring its negligible negative tail gives the stated untruncated Gaussian approximation.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [2](../../2.md)
3. [Paper 219](../../../paper-219-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
