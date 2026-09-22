<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Put $A=(Gm/h^3)F(hk)$. The two amplitude equations have coefficient matrix

$$
\begin{pmatrix}s^2-3\Omega^2+A&-2\Omega s\\2\Omega s&s^2-2A\end{pmatrix}.
$$

Its determinant gives the [dispersion relation](../../../../../../dispersion-relation.md)

$$
\boxed{s^4+(\Omega^2-A)s^2+2A(3\Omega^2-A)=0.}
$$

Writing $q=A/\Omega^2\ge0$, its squared growth rates are

$$
\boxed{\frac{s_\pm^2}{\Omega^2}=\frac{q-1\pm\sqrt{9q^2-26q+1}}2,}
$$

and the four growth rates are both [square roots](../../../../../../square-root.md) of each displayed value. Define

$$
q_- =\frac{13-4\sqrt{10}}9,\qquad q_+ =\frac{13+4\sqrt{10}}9.
$$

For $0<q<q_-$, the [discriminant](../../../../../../discriminant.md) is positive, the sum of the squared rates is $q-1<0$, and their product is $2q(3-q)>0$; both squared rates are negative. These modes have purely imaginary $s$. For $q_-<q<q_+$, the squared rates form a nonreal [complex conjugate](../../../../../../complex-conjugate.md) pair; their [square roots](../../../../../../square-root.md) include roots with positive real part. This is [overstability](../../../../../../overstability.md), meaning growing oscillations. For $q\ge q_+$, at least the plus squared rate is positive because $q>1$, so a real growing root exists. Consequently every $q>q_-$ is exponentially unstable.

Take the maximizing mode $hk=\pi$, so $q=(Gm/(h^3\Omega^2))F(\pi)$. It is unstable whenever

$$
\boxed{\frac{Gm}{h^3\Omega^2}>\frac{13-4\sqrt{10}}{9F(\pi)}.}
$$

This is also the threshold for the onset of exponential growth among all lattice modes, since $0\le F\le F(\pi)$. At equality the maximizing mode has repeated imaginary roots and can have algebraic growth; it is a marginal collision of oscillatory modes, not a strict-decay assertion. The $k=0$ mode has $F=0$, an [epicyclic motion](../../../../../../epicyclic-motion.md) sector and a zero-frequency [epicyclic guiding center](../../../../../../epicyclic-guiding-center.md) sector with possible secular shear drift. These neutral or algebraic behaviors are distinct from the strict exponential instability established by the requested inequality.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 321](../../../paper-321-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
