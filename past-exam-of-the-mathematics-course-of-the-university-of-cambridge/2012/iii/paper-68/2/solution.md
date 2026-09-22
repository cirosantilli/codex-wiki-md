<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The [symbol class](../../../../../symbol-class.md) $\mathrm{Sym}(X,\mathbb R^k;N)$ consists of smooth amplitudes with estimates

$$
\boxed{|\partial_x^\alpha\partial_\theta^\beta a(x,\theta)|\leq C_{K,\alpha,\beta}\langle\theta\rangle^{N-|\beta|},\qquad x\in K\Subset X.}
$$

There is no loss of symbol order under an $x$ [derivative](../../../../../derivative.md). A [phase function](../../../../../phase-function.md) is real and smooth for $\theta\ne0$, positively homogeneous of degree one in $\theta$, with its full differential $(d_x\Phi,d_\theta\Phi)$ nowhere zero there, at least on the amplitude's conic support. Homogeneous phases need not be smooth at $\theta=0$; that bounded-frequency region is handled separately or the amplitude is cut off near it.

Choose $\rho\in C_c^\infty(\mathbb R^k)$ equal to one near zero. The [oscillatory integral](../../../../../oscillatory-integral.md) is defined by regularization in [distributions](../../../../../distribution-mathematical-analysis.md):

$$
\boxed{\langle I_\Phi(a),f\rangle=\lim_{\varepsilon\downarrow0}\int_X\int e^{i\Phi(x,\theta)}a(x,\theta)\rho(\varepsilon\theta)f(x)\,d\theta\,dx,\qquad f\in C_c^\infty(X).}
$$

This is an ordinary integral when decay makes it absolutely convergent. For general order, the definition is independent of the regularizer. To see the mechanism, at large $|\theta|$ set

$$
A=|d_x\Phi|^2+|\theta|^2|d_\theta\Phi|^2,\qquad L=\frac{d_x\Phi\cdot\partial_x+|\theta|^2d_\theta\Phi\cdot\partial_\theta}{iA}.
$$

Homogeneity and the nonvanishing full differential give $A\gtrsim|\theta|^2$ on compact $x$ sets, and $Le^{i\Phi}=e^{i\Phi}$. Its $x$-derivative coefficients have order $-1$ and its $\theta$-derivative coefficients order zero, so each formal transpose $L^t$ lowers the amplitude order by one. Iterating more than $N+k$ times makes the test-function pairing integrable, and the same estimates control regularizer [derivatives](../../../../../derivative.md). This justifies the [cutoff function](../../../../../cutoff-function.md) limit and its independence. A fixed bounded-frequency integral is smooth in $x$.

The [singular support](../../../../../singular-support.md) of a [distribution](../../../../../distribution-mathematical-analysis.md) is the complement of the largest [open set](../../../../../open-set.md) on which it is represented by a smooth function. For the support-sensitive bound one must use [conic support of an oscillatory amplitude](../../../../../conic-support-of-an-oscillatory-amplitude.md): a closed set of limiting high-frequency directions, locally in the base variable. One sufficient precise choice is

$$
C_a=\bigcap_{R>0}\overline{\{(x,\theta/|\theta|):(x,\theta)\in\operatorname{supp}_{X\times\mathbb R^k}a,\ |\theta|\geq R\}}\subset X\times S^{k-1},
$$

with closure taken in this product. If $x_0$ is outside the projection of $C_a\cap\{d_\theta\Phi=0\}$, compactness of the [unit sphere](../../../../../unit-sphere.md) gives a neighborhood of $x_0$ and a positive uniform lower bound on $|d_\theta\Phi|$ wherever the large-frequency amplitude is supported. On that region use

$$
L_\theta=\frac{d_\theta\Phi\cdot\partial_\theta}{i|d_\theta\Phi|^2},\qquad L_\theta e^{i\Phi}=e^{i\Phi}.
$$

Its coefficients have order zero and its transpose lowers order by one. To prove $C^j$ regularity, first differentiate $j$ times in $x$, raising the amplitude order by at most $j$, and then integrate by parts more than $N+j+k$ times. The resulting integrals and their [derivatives](../../../../../derivative.md) converge uniformly on compact neighborhoods. Since $j$ is arbitrary, the [stationary-direction bound for singular support](../../../../../stationary-direction-bound-for-singular-support.md) follows:

$$
\boxed{\operatorname{sing\,supp}I_\Phi(a)\subset\pi_X\bigl(C_a\cap\{d_\theta\Phi=0\}\bigr).}
$$

This is the standard conic interpretation of the support restriction in the question; directions at infinity, rather than finite-frequency stationary points, determine possible singularities.

**If $\operatorname{supp}a(x,\cdot)$ literally means the support of the restricted function, the printed inclusion can fail.** There is a [slice-support obstruction for oscillatory singularities](../../../../../slice-support-obstruction-for-oscillatory-singularities.md). In one dimension, take $\Phi=x\theta$ and $a=x\eta(\theta)/|\theta|$, where $\eta$ is smooth and even, zero for $|\theta|\leq1$, and one for $|\theta|\geq2$. This is a symbol of order $-1$, and the full phase differential is nonzero for $\theta\ne0$. Its regularized integral near $x=0$ is

$$
I(x)=2x\int_0^\infty\eta(\theta)\frac{\cos(x\theta)}\theta\,d\theta=-2x\log|x|+\text{a smooth function}.
$$

Indeed substitute $u=|x|\theta$ in the tail, split at $u=1$, and write $\cos u=1+(\cos u-1)$ below one. The first term gives $-\log|x|$, while the remainder has an even convergent power series in $x$ plus a constant; the bounded-frequency correction is smooth. Thus $0$ is in the [singular support](../../../../../singular-support.md), but $a(0,\cdot)=0$ has empty slice support. The joint closed conic support retains this limiting base point and makes the proved theorem valid. No nonstationarity conclusion is inferred just from the amplitude vanishing at one base point.

For the [wave equation](../../../../../wave-equation-split.md), Fourier transformation in $x$ reduces the initial-value problem to $\partial_t^2\widehat E+c^2|\xi|^2\widehat E=0$, with $\widehat E(\xi,0)=0$ and $\partial_t\widehat E(\xi,0)=1$. For $c>0$ its solution is

$$
\boxed{\widehat E(\xi,t)=\frac{\sin(ct|\xi|)}{c|\xi|},}
$$

with value $t$ at zero. Choose $\chi\in C_c^\infty(\mathbb R^n)$ equal to one near zero. The [low-frequency decomposition of the wave propagator](../../../../../low-frequency-decomposition-of-the-wave-propagator.md) is

$$
E(x,t)=E_{\mathrm{low}}(x,t)+I_{\Phi_+}(a_+)(x,t)+I_{\Phi_-}(a_-)(x,t),
$$

where

$$
E_{\mathrm{low}}=(2\pi)^{-n}\int e^{ix\cdot\xi}\chi(\xi)\frac{\sin(ct|\xi|)}{c|\xi|}\,d\xi,\quad\Phi_\pm=x\cdot\xi\pm ct|\xi|,\quad a_\pm=\pm\frac{(2\pi)^{-n}(1-\chi(\xi))}{2ic|\xi|}.
$$

The low-frequency term is an ordinary smooth function: the sine quotient extends smoothly in $\xi$ at zero and all [derivatives](../../../../../derivative.md) are integrable on the fixed compact frequency set. The high-frequency amplitudes belong to $\mathrm{Sym}(\mathbb R^{n+1},\mathbb R^n;-1)$, vanish near zero, and the phases have nonzero full differential since $d_x\Phi_\pm=\xi\ne0$. Their stationary-direction equations are $x\pm ct\xi/|\xi|=0$. Such a direction can occur only if $|x|=c|t|$. The smooth low-frequency term contributes no [singular support](../../../../../singular-support.md), so

$$
\boxed{\operatorname{sing\,supp}E\subset\{(x,t):|x|=c|t|\}.}
$$

This is a statement about [singular support](../../../../../singular-support.md): some dimensions have a smooth nonzero tail inside the cone, so it does not claim that the [distribution](../../../../../distribution-mathematical-analysis.md) is concentrated only on the cone.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 68](../../paper-68-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
