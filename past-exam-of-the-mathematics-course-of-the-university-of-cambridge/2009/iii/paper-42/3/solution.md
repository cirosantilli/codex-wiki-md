<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Use [left Grassmann derivatives](../../../../../left-grassmann-derivative.md) and define the [supersymmetric covariant derivatives](../../../../../supersymmetric-covariant-derivative.md) $D_\pm=\partial_{\theta^\pm}-i\theta^\pm\partial_\pm$. Multiplication in the indicated order gives exactly the printed differential operator:

$$
iD_-D_+=i\partial_{\theta^-}\partial_{\theta^+}+\theta^-\partial_{\theta^+}\partial_- -\theta^+\partial_{\theta^-}\partial_+ -i\theta^-\theta^+\partial_-\partial_+.
$$

Thus the equation is $iD_-D_+\Phi=W(\Phi)$ in [two-dimensional N=(1,1) superspace](../../../../../two-dimensional-n-1-1-superspace.md).

Under a [Lorentz boost](../../../../../lorentz-boost.md), take $x^\pm\mapsto e^{\pm\omega}x^\pm$ and $\theta^\pm\mapsto e^{\pm\omega/2}\theta^\pm$. The derivatives $\partial_\pm$ have boost weights $\mp1$, and $D_\pm$ have weights $\mp1/2$. Consequently $D_-D_+$ has weight zero, and is a [Lorentz scalar](../../../../../lorentz-scalar.md). Both $\Phi$ and the ordinary function $W(\Phi)$ are scalar [superfields](../../../../../superfield.md), so the equation is [Lorentz invariant](../../../../../lorentz-invariance.md).

For [supersymmetry](../../../../../supersymmetry-split.md), $\{\partial_\theta,\theta\}=1$ and anticommutation of distinct odd coordinates give

$$
\{D_s,Q_t\}=0\quad(s,t\in\{+,-\}),\qquad Q_\pm^2=i\partial_\pm,\qquad \{Q_+,Q_-\}=0.
$$

Moving either [supercharge](../../../../../supersymmetry-generator.md) through the two odd derivatives introduces two minus signs, hence $[Q_t,D_-D_+]=0$. If $\delta\Phi=\epsilon^+Q_+\Phi+\epsilon^-Q_-\Phi$, with odd constant parameters, the [chain rule](../../../../../chain-rule.md) for an even scalar [superfield](../../../../../superfield.md) gives

$$
\delta\bigl(iD_-D_+\Phi-W(\Phi)\bigr)=\sum_{t=\pm}\epsilon^tQ_t\bigl(iD_-D_+\Phi-W(\Phi)\bigr).
$$

Therefore a solution is mapped to a solution, proving [supersymmetry](../../../../../supersymmetry-split.md) invariance.

To compute the [supersymmetric Liouville equation](../../../../../supersymmetric-liouville-equation.md), order the odd coordinates as $\theta^-\theta^+$ and anticommute the fermionic component fields with both coordinates. In particular, $\partial_{\theta^+}(\theta^-\theta^+)=-\theta^-$. Direct application of the operator gives

$$
iD_-D_+\Phi=F+i\theta^-\partial_-\psi_- -i\theta^+\partial_+\psi_+ -i\theta^-\theta^+\partial_-\partial_+\phi.
$$

Let $N=\Phi-\phi$. Only the two products of its degree-one terms survive in $N^2$; for example, $(i\theta^-\psi_+)(i\theta^+\psi_-)=\theta^-\theta^+\psi_+\psi_-$. Hence $N^2=2\theta^-\theta^+\psi_+\psi_-$ and $N^3=0$. The [exponential function](../../../../../exponential-function.md) expands exactly as

$$
e^\Phi=e^\phi\left[1+i\theta^-\psi_++i\theta^+\psi_-+\theta^-\theta^+(iF+\psi_+\psi_-)\right].
$$

Equating the constant terms fixes the [auxiliary field](../../../../../auxiliary-field.md), $\boxed{F=e^\phi}$. The linear and quadratic terms then give the requested component field [equations of motion](../../../../../equation-of-motion.md):

$$
\boxed{\partial_-\psi_-=e^\phi\psi_+,\qquad \partial_+\psi_+=-e^\phi\psi_-,\qquad \partial_-\partial_+\phi=-e^{2\phi}+ie^\phi\psi_+\psi_-.}
$$

The signs here follow from the printed operator, the printed component expansion, and [left Grassmann derivatives](../../../../../left-grassmann-derivative.md); no convention change has been made in eliminating the [auxiliary field](../../../../../auxiliary-field.md).

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 42](../../paper-42-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
