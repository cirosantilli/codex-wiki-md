<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the [Fourier transform](../../../../fourier-transform-split.md) convention $\phi(x)=\int d^4p/(2\pi)^4\,e^{-ip\cdot x}\widetilde\phi(p)$, and similarly for $\Phi$. All [four-momenta](../../../../four-momentum.md) at an [interaction vertex](../../../../interaction-vertex.md) are incoming. The quadratic terms are diagonal, so the [scalar propagators](../../../../scalar-propagator.md) are

$$
\boxed{D_\phi(p)=\frac{i}{p^2-m^2+i0},\qquad
D_\Phi(p)=\frac{i}{p^2-M^2+i0},\qquad D_{\phi\Phi}=0.}
$$

The [field interaction terms](../../../../field-interaction-term.md) are $\lambda\phi\Phi^2/2$ and $g\Phi\partial_\mu\phi\partial^\mu\phi/2$. The two identical field slots cancel the factor $1/2$ at either cubic [interaction vertex](../../../../interaction-vertex.md). Expanding $\exp(iS_{\rm int})$ therefore gives

$$
\boxed{\begin{aligned}
\phi(p)\Phi(k)\Phi(\ell):&\quad i\lambda,\qquad p+k+\ell=0,\\
\Phi(k)\phi(p)\phi(q):&\quad -ig\,p\cdot q,\qquad k+p+q=0.
\end{aligned}}
$$

In the second rule $p,q$ are specifically the two $\phi$ [four-momenta](../../../../four-momentum.md); there is no derivative acting on the $\Phi$ leg. Indeed the two derivatives give $(-ip_\mu)(-iq^\mu)=-p\cdot q$, fixing the minus sign. This is a [mixed scalar derivative cubic vertex](../../../../mixed-scalar-derivative-cubic-vertex.md). For arbitrary off-shell legs one may equivalently write $-ig(k^2-p^2-q^2)/2$, but may not replace the squared [four-momenta](../../../../four-momentum.md) by squared [masses](../../../../mass.md) unless those legs are on their [mass shells](../../../../mass-shell.md).

Each [interaction vertex](../../../../interaction-vertex.md) also carries $(2\pi)^4\delta^{(4)}(\sum p)$ for [momentum conservation](../../../../momentum-conservation.md). Integrate independent [loop momenta](../../../../loop-momentum.md) with $d^4p/(2\pi)^4$ and divide by the [Feynman-diagram symmetry factor](../../../../feynman-diagram-symmetry-factor.md). An amputated external scalar leg has factor 1. The [Feynman i-epsilon prescription](../../../../feynman-i-epsilon-prescription.md) fixes the propagator poles. As a dimensional check in four spacetime dimensions, $[\phi]=[\Phi]=1$, $[\lambda]=1$ and $[g]=-1$ in [mass dimensions](../../../../mass-dimension.md); the two powers of [momentum](../../../../momentum-split.md) in the derivative rule restore [mass dimension](../../../../mass-dimension.md) one for its cubic [interaction vertex](../../../../interaction-vertex.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [2019](../../../2019-split.md)
4. [Past exam of the quantum field theory course of the University of Oxford](../../../split.md)
5. [Quantum field theory course of the University of Oxford](../../../../quantum-field-theory-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
