<h1 id="j/j2/solution">Solution</h1>

↑ **Parent:** [J2](../j2.md)

In vacuum, the source-free [Maxwell equations](../../../../maxwell-equations-split.md) are $\nabla\cdot E=\nabla\cdot B=0$, $\nabla\times E=-\partial_tB$ and $\nabla\times B=c^{-2}\partial_tE$. Put $\vartheta=\omega(t-z/c)$ and denote the field amplitude by $E_0$. The corresponding travelling-wave [magnetic field](../../../../magnetic-field-split.md) is

$$
\boxed{B=\frac{E_0}{c}(-\sin\vartheta,\cos\vartheta,0)}.
$$

Both divergences vanish because the fields have no longitudinal component and no dependence on the transverse coordinates. Direct differentiation gives $\nabla\times E=(\omega E_0/c)(\cos\vartheta,\sin\vartheta,0)=-\partial_tB$ and $\nabla\times B=(\omega E_0/c^2)(-\sin\vartheta,\cos\vartheta,0)=c^{-2}\partial_tE$.

Introducing potentials by $B=\nabla\times A$ and $E=-\nabla\phi-\partial_tA$ automatically satisfies the magnetic-divergence and Faraday equations. The remaining [Maxwell equations](../../../../maxwell-equations-split.md) become equations for these potentials, with the usual gauge freedom. For $\omega\ne0$ take $\phi=0$ and

$$
A=\frac c\omega B=\frac{E_0}{\omega}(-\sin\vartheta,\cos\vartheta,0).
$$

Differentiation verifies both potential relations.

The electromagnetic force is $Q(E+v\times B)$. Confinement also supplies a normal reaction force. For motion in a plane of constant $z$, both $v$ and $B$ are tangent to the plane, so their cross product is normal and is balanced by that reaction. It does not enter the in-plane equation $m\ddot r=QE_0(\cos\vartheta,\sin\vartheta)$.

At the fixed plane, the solution with no uniform drift is

$$
r(t)=r_0-\frac{QE_0}{m\omega^2}(\cos\vartheta,\sin\vartheta).
$$

It is circular, with

$$
\boxed{R=\frac{|QE_0|}{m\omega^2}}.
$$

Other initial data can add a constant drift velocity; the question only asks for the possibility of circular motion.

## ↑ Ancestors (12)

1. [J2](../j2.md)
2. [J](../../j.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the options II course of the University of Oxford](../../../split.md)
5. [Options II course of the University of Oxford](../../../../options-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
