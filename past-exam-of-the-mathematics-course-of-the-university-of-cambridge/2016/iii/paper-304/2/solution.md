<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Use [Lie algebra](../../../../../lie-algebra-split.md) generators with $[T_b,T_c]=f^a{}_{bc}T_a$, and define the adjoint [gauge covariant derivative](../../../../../gauge-covariant-derivative.md) by $(D_\mu X)^a=\partial_\mu X^a+f^a{}_{bc}A_\mu^bX^c$. Varying the [gauge field strength](../../../../../gauge-field-strength.md) gives $\delta F_{\mu\nu}=D_\mu\delta A_\nu-D_\nu\delta A_\mu$. Antisymmetry followed by [integration by parts](../../../../../integration-by-parts.md) therefore gives

$$
\delta S=\frac1{g^2}\int F^{a\mu\nu}(D_\mu\delta A_\nu)^a\,d^4x=-\frac1{g^2}\int(D_\mu F^{\mu\nu})^a\delta A_\nu^a\,d^4x.
$$

For variations vanishing at the boundary, **the [Yang-Mills equations](../../../../../yang-mills-equations.md)** are

$$
\boxed{(D_\mu F^{\mu\nu})^a=0.}
$$

The [Jacobi identity](../../../../../jacobi-identity.md) for the commutators of [gauge covariant derivatives](../../../../../gauge-covariant-derivative.md), using $[D_\mu,D_\nu]X=[F_{\mu\nu},X]$, gives **the [gauge-theory Bianchi identity](../../../../../gauge-theory-bianchi-identity.md)**:

$$
\boxed{D_\mu F_{\nu\rho}+D_\nu F_{\rho\mu}+D_\rho F_{\mu\nu}=0,\qquad D_\mu\widetilde F^{\mu\nu}=0.}
$$

In the second form of the [gauge-theory Bianchi identity](../../../../../gauge-theory-bianchi-identity.md) $\widetilde F^{\mu\nu}=\tfrac12\varepsilon^{\mu\nu\rho\sigma}F_{\rho\sigma}$. The identity is a geometric consequence of the definition of curvature, not a second dynamical field equation.

For the usual non-Abelian [Yang-Mills theory](../../../../../yang-mills-theory.md), the quantum [running coupling](../../../../../running-coupling.md) becomes strong at low energies. [Dimensional transmutation](../../../../../dimensional-transmutation.md) generates a scale absent from the classically scale-invariant equations. The expected confining dynamics and massive colour-singlet spectrum involve [confinement](../../../../../confinement.md) and a [mass gap](../../../../../mass-gap.md), rather than freely propagating weakly coupled coloured waves. These nonperturbative effects are not captured by simply solving the classical equations; this is not a claim of a mathematical proof of the Yang-Mills [mass gap](../../../../../mass-gap.md).

Write the gauge condition as $\chi^a[A]=f^a[A]$ to distinguish it from the [structure constants](../../../../../structure-constant.md). Under an infinitesimal [gauge transformation](../../../../../gauge-transformation.md), $\delta_\omega A_\mu=D_\mu\omega$. Define the [Faddeev-Popov operator](../../../../../faddeev-popov-operator.md) by $\mathcal M^{ab}=\delta\chi^a[A+D\omega]/\delta\omega^b|_{\omega=0}$. In a Euclidean convention, **the gauge-fixing and ghost additions** can be chosen as

$$
\boxed{S_{gf}=\frac1{2\xi g^2}\int d^4x\,\chi^a\chi^a,\qquad S_{gh}=\int d^4x\,\overline c^{\,a}\mathcal M^{ab}c^b.}
$$

A nonlocal kernel would require a double integral; a local functional $\chi$ instead makes $\mathcal M$ a local differential operator. Choosing a local gauge functional thus retains a local [gauge-fixed action](../../../../../gauge-fixed-action.md) and the ordinary local interaction structure of [perturbative quantum field theory](../../../../../perturbative-quantum-field-theory-split.md).

The fields $c^a$ and $\overline c^{\,a}$ are independent [Grassmann-valued fields](../../../../../grassmann-field.md) in the [Adjoint representation](../../../../../adjoint-representation-of-a-lie-algebra.md), Lorentz scalars with [ghost numbers](../../../../../ghost-number.md) $+1$ and $-1$. They are the [Faddeev-Popov ghost fields](../../../../../faddeev-popov-ghost.md): their functional integral produces $\det\mathcal M$, the [Faddeev-Popov determinant](../../../../../faddeev-popov-determinant.md) correcting the volume element along a [gauge orbit](../../../../../gauge-orbit.md). They are internal fields, not physical asymptotic particles. Their statistics supply a minus sign for every closed [ghost loop](../../../../../ghost-loop.md). No auxiliary field is needed in the displayed gauge-fixing representation.

In [axial gauge](../../../../../axial-gauge.md), $\chi^a=n^\mu A_\mu^a$, so

$$
\mathcal M^{ac}=n\cdot\partial\,\delta^{ac}+f^a{}_{bc}\,n^\mu A_\mu^b,
\qquad S_{gh}=\int d^4x\,[\overline c^{\,a}n\cdot\partial c^a+f^a{}_{bc}\overline c^{\,a}n^\mu A_\mu^bc^c].
$$

With the [Fourier transform](../../../../../fourier-transform.md) convention $e^{ik\cdot x}$, **the ghost Feynman rules** in the original normalization of $A$ are

$$
\boxed{\langle c^a(k)\overline c^{\,b}(-k)\rangle_0=\frac{\delta^{ab}}{i\,n\cdot k},\qquad V_{\overline c^a A_\mu^b c^c}=-f^a{}_{bc}n_\mu.}
$$

Momentum conservation accompanies the vertex; each [ghost loop](../../../../../ghost-loop.md) has the extra minus sign. With a canonically normalized field $A=gA_{\mathrm{can}}$, the vertex is instead $-g f^a{}_{bc}n_\mu$. The [gauge fixing](../../../../../gauge-fixing.md) term is quadratic and introduces no further interaction vertex.

The Euclidean quadratic kernel of $A$ is $g^{-2}[k^2\delta_{\mu\nu}-k_\mu k_\nu+\xi^{-1}n_\mu n_\nu]$. For $n\cdot k\ne0$, its inverse is

$$
D_{\mu\nu}^{ab}(k)=\frac{g^2\delta^{ab}}{k^2}\left[\delta_{\mu\nu}-\frac{k_\mu n_\nu+n_\mu k_\nu}{n\cdot k}+\frac{(n^2+\xi k^2)k_\mu k_\nu}{(n\cdot k)^2}\right].
$$

This follows by multiplication with the kernel: the $k^2\delta-kk$ piece gives $I-nk^T/(n\cdot k)$, and the $\xi^{-1}nn$ piece supplies the missing $nk^T/(n\cdot k)$. **The strict [axial-gauge propagator](../../../../../axial-gauge-propagator.md)** is therefore

$$
\boxed{D_{\mu\nu}^{ab}(k)\big|_{\xi=0}=\frac{g^2\delta^{ab}}{k^2}\left[\delta_{\mu\nu}-\frac{k_\mu n_\nu+n_\mu k_\nu}{n\cdot k}+\frac{n^2 k_\mu k_\nu}{(n\cdot k)^2}\right].}
$$

It obeys $n^\mu D_{\mu\nu}=0$. Every ghost attachment to an internal gauge propagator therefore vanishes in the strict limit; equivalently, $\mathcal M=n\cdot\partial$ on the gauge slice. Thus the interacting [Faddeev-Popov ghosts](../../../../../faddeev-popov-ghost.md) decouple. Residual gauge transformations and the poles at $n\cdot k=0$ require compatible boundary conditions and an [axial-gauge pole prescription](../../../../../axial-gauge-pole-prescription.md).

After [Wick rotation](../../../../../wick-rotation.md), the corresponding Minkowski propagator has $\delta_{\mu\nu}$ replaced by $\eta_{\mu\nu}$ and the usual overall factor $-i$, with a compatible causal prescription. The fixed $n$ makes the gauge-fixed propagator nonmanifestly Lorentz covariant. Nevertheless, [gauge invariance](../../../../../gauge-invariance.md) makes physical observables independent of this gauge-choice vector, so their perturbative predictions are [Lorentz invariant](../../../../../lorentz-invariance.md). Already at tree level, contraction with conserved external currents removes all terms containing $k_\mu$ or $k_\nu$, leaving $g^2j\cdot j'/k^2$. The quantum [Ward identities](../../../../../ward-identity.md) give the analogous cancellation in complete physical amplitudes; arbitrary gauge-dependent Green functions need not be independent of $n$.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 304](../../paper-304-split.md)
3. [Iii](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
