<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Treat the left side as a causal [convolution](../../../../convolution.md) with $t^{-\alpha}$. Under the usual Laplace-transform hypotheses, the [convolution theorem for Laplace transforms](../../../../convolution-theorem-for-laplace-transforms.md) gives

$$
\widehat\Phi(s)\,\Gamma(1-\alpha)s^{\alpha-1}=\widehat f(s).
$$

For an absolutely continuous $f$ with $f(0)=0$, the [derivative](../../../../derivative.md) transform is $\mathcal L[f']=s\widehat f$. Consequently

$$
\widehat\Phi(s)=\frac{s^{-\alpha}}{\Gamma(1-\alpha)}\mathcal L[f'](s).
$$

Since $\mathcal L[t^{\alpha-1}]=\Gamma(\alpha)s^{-\alpha}$, inverting the product proves

$$
\boxed{\Phi(t)=\frac1{\Gamma(\alpha)\Gamma(1-\alpha)}\int_0^tf'(\tau)(t-\tau)^{\alpha-1}d\tau.}
$$

Here $0<\alpha<1$ makes both power kernels locally integrable. For example assume exponential growth bounds sufficient for the transforms and a regularity class where the [convolution](../../../../convolution.md) is defined. This is the [Abel integral equation of fractional order](../../../../abel-integral-equation-of-fractional-order.md); the initial value removes the extra boundary term in the [derivative](../../../../derivative.md) transform.

For $f(t)=t$, the remaining integral is $\int_0^t(t-\tau)^{\alpha-1}d\tau=t^\alpha/\alpha$. Thus

$$
\boxed{\Phi(t)=\frac{t^\alpha}{\Gamma(\alpha+1)\Gamma(1-\alpha)}.}
$$

Substitution into the original equation checks the result: scaling $\tau=tu$ gives $t\,B(\alpha+1,1-\alpha)/[\Gamma(\alpha+1)\Gamma(1-\alpha)]=t$ by the [beta-gamma identity](../../../../beta-gamma-identity.md).

## ↑ Ancestors (12)

1. [5](../5.md)
2. [Paper 2](../../paper-2-split.md)
3. [2009](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
