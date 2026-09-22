<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

The proposed [change of variables](../../../change-of-variables-formula.md) gives $u=x-3y$, $v=2x+y$, with inverse $x=(u+3v)/7$, $y=(v-2u)/7$. The [Jacobian determinant](../../../jacobian-determinant.md) is

$$
\frac{\partial(u,v)}{\partial(x,y)}=7,\qquad \left|\frac{\partial(x,y)}{\partial(u,v)}\right|=\frac17.
$$

The two lines of slope $-2$ become $v=1,4$, while the two lines of slope $1/3$ become $u=0,7$. Thus the parallelogram becomes $0\leq u\leq7$, $1\leq v\leq4$. Since $v$ stays positive, the transformed integrand has no singularity there. The [double integral](../../../double-integral.md) is

$$
\boxed{\iint_D\frac{x-3y}{2x+y}\,dx\,dy=\frac17\int_0^7u\,du\int_1^4\frac{dv}{v}=\frac72\ln4=7\ln2.}
$$

## ↑ Ancestors (11)

1. [5](../5.md)
2. [2014 resit](../../2014-resit-split.md)
3. [Past exam of the mathematical methods II course of the University of Oxford](../../split.md)
4. [Mathematical methods II course of the University of Oxford](../../../mathematical-methods-ii-course-of-the-university-of-oxford.md)
5. [Year 1 of the physics course of the University of Oxford](../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
