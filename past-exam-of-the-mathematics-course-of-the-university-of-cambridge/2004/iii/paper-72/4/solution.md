<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

For [antiplane shear](../../../../../antiplane-shear.md), the infinitesimal displacement is $(0,0,w(x_1,x_2))$. The isotropic [linear elasticity](../../../../../linear-elasticity.md) constitutive law gives $\sigma_{13}=\mu w_{,1}$ and $\sigma_{23}=\mu w_{,2}$, together with the symmetric entries $\sigma_{31},\sigma_{32}$. All other [stress tensor](../../../../../cauchy-stress-tensor.md) components vanish. Static force balance without [body force](../../../../../body-force.md) becomes $\mu(w_{,11}+w_{,22})=0$, so $w$ satisfies the [Laplace equation](../../../../../laplace-equation.md).

Locally choose a [harmonic conjugate](../../../../../harmonic-conjugate.md) $\phi$ by $\phi_{,1}=w_{,2}$ and $\phi_{,2}=-w_{,1}$. Compatibility follows from the [Laplace equation](../../../../../laplace-equation.md). These are the [Cauchy-Riemann equations](../../../../../cauchy-riemann-equations.md) for $F=\phi+iw$, and hence

$$
F'(z)=\phi_{,1}+iw_{,1}=w_{,2}+iw_{,1},\qquad \boxed{\sigma_{23}+i\sigma_{13}=\mu F'(z).}
$$

Thus the [complex stress potential for antiplane shear](../../../../../complex-stress-potential-for-antiplane-shear.md) supplies both stresses and, by integration, the displacement. A global potential must have the displacement periods appropriate to the cracked body; these periods also help fix homogeneous solutions.

For the additional crack-induced field, set $G=\mu F'$ and $p(t)=\sigma_{23}^A(t,0)$. Only $p$ loads the prospective faces, since $\sigma_{13}^A$ is tangential to their normal. Denote upper and lower boundary values by $G^+,G^-$. The imposed cancellation of face [tractions](../../../../../traction.md) is $\operatorname{Re}G^\pm=-p$. The traction data and geometry are invariant under the displacement reflection $w(x_1,x_2)\mapsto-w(x_1,-x_2)$. For the induced correction with no independently added loading, uniqueness up to a rigid translation allows the odd displacement choice. Then $w_{,2}$ is even, $w_{,1}$ is odd, and $G^-=\overline{G^+}$ on the real axis. Therefore the [Hilbert problem for an antiplane crack](../../../../../hilbert-problem-for-an-antiplane-crack.md) is

$$
\boxed{G^++G^-=-2p\text{ on cracks},\qquad G^+-G^-=0\text{ on intact portions}.}
$$

The second condition expresses continuation through uncracked material. There $G$ is real and the additional $\sigma_{13}$ vanishes. This scalar [Riemann-Hilbert problem](../../../../../riemann-hilbert-problem.md) is supplemented by at most inverse-square-root stress singularities at the crack tips and the usual correction with no additional remote resultant or imposed dislocation. Without a far-field or period normalization, the face conditions alone permit homogeneous terms. The formulas below select this normalized induced field and explicitly identify the excluded terms.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 72](../../paper-72-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
