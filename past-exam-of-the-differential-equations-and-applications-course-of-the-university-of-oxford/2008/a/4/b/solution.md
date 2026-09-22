<h1 id="a/4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Try $\rho=t^af(\eta)$, $\eta=x/t^b$. The boundary data force $a=3$ and $f(0)=1$. The time [derivative](../../../../../derivative.md) scales as $t^{a-1}$, advection as $t^{2a-b}$ and the source as $t^{a+c}$. Balancing all three gives $c=-1$ and $b=a+1=4$. Substitution then yields

$$
3f-4\eta f'+ff'=f,\qquad
\boxed{c=-1,\quad\eta=x/t^4,\quad(f-4\eta)f'+2f=0,\quad f(0)=1.}
$$

For the pointwise initial trace at any fixed $x>0$, the far-profile requirement is $f(\eta)=o(\eta^{3/4})$ as $\eta\to\infty$ on any smooth branch extending that far; a compact-support continuation also meets it. Solving or selecting a [shock](../../../../../shock-wave.md) continuation was not required. The time-dependent source is singular at $t=0$, so the similarity reduction is stated on $t>0$.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [4](../../4.md)
3. [A](../../../a.md)
4. [2008](../../../../2008-split.md)
5. [Past exam of the differential equations and applications course of the University of Oxford](../../../../split.md)
6. [Differential equations and applications course of the University of Oxford](../../../../../differential-equations-and-applications-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
