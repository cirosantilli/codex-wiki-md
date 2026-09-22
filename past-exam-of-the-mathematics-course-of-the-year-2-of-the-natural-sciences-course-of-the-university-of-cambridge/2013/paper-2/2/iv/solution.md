<h1 id="2/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

A positive matching root $x_*$ gives $s=x_*^2/R^2$. Substituting the root value requested by the question gives the intended expression

$$
\boxed{s_{\rm intended}=\frac{\pi^2}{R^2}.}
$$

After the index correction in part (iii), this is indeed the lowest mode in the $\ell=1$ sector, because its condition is $j_0(x)=\sin x/x=0$ and its first positive root is $\pi$. It is also the minimum over $\ell\geq1$.

However, **the literal scalar problem includes $\ell=0$**, for which matching gives $\cos x=0$. Its first positive root is $\pi/2$, so the actual minimum for the written scalar equations and stated boundary conditions is

$$
\boxed{s_{\rm scalar,min}=\frac{\pi^2}{4R^2}.}
$$

An explicit counterexample to the larger proposed minimum is $B_{\rm in}=j_0(\pi r/(2R))$, $B_{\rm out}=2R/(\pi r)$, with no angular dependence. At $R$, both values are $2/\pi$ and both radial derivatives are $-2/(\pi R)$.

To verify minimality, put $u=rF_\ell$. The radial problem is $-u''+\ell(\ell+1)u/r^2=su$, $u(0)=0$, $u'(R)+\ell u(R)/R=0$. Its [Rayleigh quotient](../../../../../rayleigh-quotient.md) is

$$
s=\frac{\int_0^R[|u'|^2+\ell(\ell+1)|u|^2/r^2]dr+\ell|u(R)|^2/R}{\int_0^R|u|^2dr}.
$$

For $\ell=0$ this is the Dirichlet-Neumann interval problem, whose lowest eigenvalue is $\pi^2/(4R^2)$. The additional nonnegative terms increase with $\ell$, proving the scalar minimum and the minimum-at-$\ell=1$ statement for the restricted family. A monopole-free magnetic multipole interpretation would exclude $\ell=0$ and yield the intended value, but that extra restriction is not supplied by the stated scalar model. The claim about the first zero is not valid for every $f_\ell$ as printed.

## ↑ Ancestors (13)

1. [Iv](../iv.md)
2. [2](../../2.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
