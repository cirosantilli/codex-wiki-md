<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Apply [Green's second identity](../../../../../green-second-identity.md) to $\Phi(\mathbf r)$ and $G(\mathbf r,\mathbf r')$, differentiating in $\mathbf r$:

$$
\int_V(\Phi\Delta G-G\Delta\Phi)\,dV
=\int_S\left(\Phi\frac{\partial G}{\partial n}-G\frac{\partial\Phi}{\partial n}\right)dS.
$$

The volume terms become $\Phi(\mathbf r')-\int_VG\rho\,dV$. On the boundary $G=0$ and $\Phi=f$, so

$$
\boxed{\Phi(\mathbf r')=\int_V\rho(\mathbf r)G(\mathbf r,\mathbf r')\,dV
+\int_S f(\mathbf r)\frac{\partial G}{\partial n}(\mathbf r,\mathbf r')\,dS}.
$$

Here $\partial/\partial n$ is the outward [normal derivative](../../../../../normal-derivative.md) in the integration variable. One may justify the identity at the singularity by excising a small sphere around $\mathbf r'$; its unit flux supplies the evaluation $\Phi(\mathbf r')$.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
