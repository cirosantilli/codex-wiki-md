<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use the angular-frequency [Fourier transform](../../../../../../fourier-transform.md) convention

$$
\widehat f(\lambda)=\int_{\mathbb R}f(x)e^{-i\lambda x}\,dx.
$$

A precise sufficient interpretation of the regularity assumption is $f\ne0$, $f\in H^1(\mathbb R)$ in the [first-order Sobolev space](../../../../../../first-order-sobolev-space.md) and $xf\in L^2(\mathbb R)$; in particular, nonzero [Schwartz functions](../../../../../../schwartz-function.md) are admissible. We use the [Plancherel theorem](../../../../../../plancherel-theorem.md), in the normalization $\|\widehat f\|_2^2=2\pi\|f\|_2^2$, together with its derivative identity $\widehat{f'}(\lambda)=i\lambda\widehat f(\lambda)$. Both identities hold in $L^2$ for $f\in H^1$, by extending their identities for [Schwartz functions](../../../../../../schwartz-function.md). Thus the frequency factor is

$$
\frac{\int\lambda^2|\widehat f(\lambda)|^2\,d\lambda}{\int|\widehat f(\lambda)|^2\,d\lambda}=\frac{\|f'\|_2^2}{\|f\|_2^2}.
$$

For a [Schwartz function](../../../../../../schwartz-function.md), [integration by parts](../../../../../../integration-by-parts.md) gives $\|f\|_2^2=-2\operatorname{Re}\int x f'(x)\overline{f(x)}\,dx$. This remains true under the stated assumptions: insert a smooth cutoff $\chi_R(x)=\chi(x/R)$ into the derivative of $x|f|^2$, where $\chi$ is one near zero and compactly supported. Integration gives

$$
\int(\chi_R+x\chi_R')|f|^2\,dx=-2\operatorname{Re}\int\chi_R x f'\overline f\,dx.
$$

The cutoff-derivative term tends to zero, since $x\chi_R'$ is bounded independently of $R$ and supported in a tail. The other terms converge by [dominated convergence](../../../../../../dominated-convergence-theorem.md) and the integrability of $|f'||xf|$, furnished by the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md). Hence

$$
\|f\|_2^2=-2\operatorname{Re}\langle f',xf\rangle\leq2|\langle f',xf\rangle|\leq2\|f'\|_2\|xf\|_2.
$$

After squaring and using the [Plancherel theorem](../../../../../../plancherel-theorem.md), we obtain the [uncentred Fourier uncertainty principle](../../../../../../uncentred-fourier-uncertainty-principle.md):

$$
\boxed{\frac{\int x^2|f(x)|^2\,dx}{\int|f(x)|^2\,dx}\frac{\int\lambda^2|\widehat f(\lambda)|^2\,d\lambda}{\int|\widehat f(\lambda)|^2\,d\lambda}\geq\frac14.}
$$

If equality holds, both displayed inequalities must be equalities. The equality condition in the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) gives $f'=cxf$ almost everywhere for a constant $c\in\mathbb C$; the real-part inequality and the identity for $\|f\|_2^2$ then force $c=-a$ with $a>0$ real. The [weak derivative](../../../../../../weak-derivative.md) equation has the solution $f(x)=C e^{-ax^2/2}$: locally multiply by $e^{ax^2/2}$ to obtain a function whose weak derivative is zero, hence a constant. Conversely, for this [Gaussian function](../../../../../../gaussian-function.md) the normalized second moments are $1/(2a)$ in position and $a/2$ in angular frequency, whose product is $1/4$. Therefore

$$
\boxed{\text{Equality holds exactly for }f(x)=C e^{-ax^2/2},\quad a>0,\ C\in\mathbb C\setminus\{0\}.}
$$

These are raw second moments, rather than variances about their respective means. Consequently translations and nonzero frequency modulations of the [Gaussian function](../../../../../../gaussian-function.md) are not equality cases here; the [equality case of the Heisenberg uncertainty relation](../../../../../../equality-case-of-the-heisenberg-uncertainty-relation.md) for centred variances has those additional freedoms.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 7](../../../paper-7-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
