<h1 id="8e/solution">Solution</h1>

↑ **Parent:** [8E](../8e.md)

For $\operatorname{Re}z>0$, absolute convergence permits the two-dimensional gamma integral

$$
\Gamma(z/2)^2=\int_0^\infty\int_0^\infty
 e^{-(u+v)}u^{z/2-1}v^{z/2-1}\,du\,dv.
$$

Put $u=rs$, $v=r(1-s)$, with $r>0$, $0<s<1$ and [Jacobian determinant](../../../../../jacobian-determinant.md) $r$. Separation of the integrals gives the [beta--gamma identity](../../../../../beta-gamma-identity.md)

$$
\boxed{\Gamma(z/2)^2=\Gamma(z)B(z/2,z/2)}.
$$

The beta integral is finite in this half-plane. Thus a zero of $\Gamma(z)$ would imply $\Gamma(z/2)=0$, and iteration would imply $\Gamma(z/2^m)=0$ for every positive integer $m$. But integration by parts gives $w\Gamma(w)=\Gamma(1+w)$, and continuity near one makes $\Gamma(1+w)\to1$ as $w\to0$. It cannot vanish for sufficiently small $w$, a contradiction. Therefore the [Gamma function has no zeros](../../../../../gamma-function-has-no-zeros.md) in the right half-plane.

For any $z$ outside the nonpositive integers, choose an integer $n$ with $\operatorname{Re}(z+n)>0$. The [Gamma function recurrence](../../../../../gamma-function-recurrence.md) gives

$$
\Gamma(z)=\frac{\Gamma(z+n)}{z(z+1)\cdots(z+n-1)}\ne0.
$$

At the excluded integers gamma has poles, with nonzero residues by the same recurrence. Hence **the meromorphic [gamma function](../../../../../gamma-function.md) has no zeros anywhere**; at its poles it has no finite value to which a nonzero-value assertion could apply.

## ↑ Ancestors (10)

1. [8E](../8e.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
