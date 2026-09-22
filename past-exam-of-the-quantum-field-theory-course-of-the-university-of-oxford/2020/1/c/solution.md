<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Define $\mathcal M$ by removing the factor $i(2\pi)^4\delta^{(4)}(p_1+p_2-p_3-p_4)$ from the connected transition [matrix element](../../../../matrix-element.md). The single [tree-level Feynman diagram](../../../../tree-level-feynman-diagram.md) in [i](../b/i.md) gives

$$
i\mathcal M=(-ig)^2\frac{i}{q^2-m^2+i0}
[\bar u_{s_3}(p_3)u_{s_1}(p_1)]
[\bar u_{s_4}(p_4)u_{s_2}(p_2)],
\qquad q=p_1-p_3.
$$

There is no identical-particle exchange term because the species differ. Each incoming [fermion](../../../../fermion.md) has two equally populated [spin angular momentum](../../../../spin.md) states in an unpolarized beam. Their probabilities multiply to $1/4$, giving a [spin average](../../../../spin-average.md) over the four initial choices. The unobserved final [spin angular momentum](../../../../spin.md) states are distinct outcomes, so their probabilities are added by a [spin sum](../../../../spin-sum.md), with no final averaging:

$$
\overline{|\mathcal M|^2}=\frac14\sum_{s_1,s_2,s_3,s_4}|\mathcal M|^2.
$$

Taking the complex conjugate of $\bar u_3u_1$ gives $\bar u_1u_3$. The [fermion spin sum](../../../../fermion-spin-sum.md) therefore converts each squared bilinear into a [gamma-matrix trace](../../../../gamma-matrix-trace.md):

$$
\overline{|\mathcal M|^2}
=\frac{g^4}{4(q^2-m^2)^2}
\operatorname{tr}[(\not p_3+m)(\not p_1+m)]
\operatorname{tr}[(\not p_4+m)(\not p_2+m)].
$$

Using $\operatorname{tr}1=4$, $\operatorname{tr}\gamma^\mu=0$, $\operatorname{tr}(\gamma^\mu\gamma^\nu)=4\eta^{\mu\nu}$, and the [mass shell](../../../../mass-shell.md) conditions $p_j^2=m^2$, each [gamma-matrix trace](../../../../gamma-matrix-trace.md) is

$$
4(p_1\cdot p_3+m^2)=4\left(2m^2-\frac{q^2}{2}\right)
=2(4m^2-q^2).
$$

The second equality follows from $q^2=2m^2-2p_1\cdot p_3$; [momentum conservation](../../../../momentum-conservation.md) gives the identical result for $p_2,p_4$. Hence

$$
\boxed{\overline{|\mathcal M|^2}
=g^4\left(\frac{4m^2-q^2}{m^2-q^2}\right)^2.}
$$

**The printed prefactor $g^2$ is incorrect for the stated coupling.** Each of the two [Yukawa interaction](../../../../yukawa-interaction.md) vertices contributes one $g$ to the [scattering amplitude](../../../../scattering-amplitude.md), so its square is proportional to $g^4$. As a concrete counterexample, take $g=2$, $m>0$, and forward elastic kinematics $p_3=p_1$, $p_4=p_2$. Then $q^2=0$ and the [spin average](../../../../spin-average.md) is $16g^4=256$, whereas the printed expression gives $16g^2=64$.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [2020](../../../2020-split.md)
4. [Past exam of the quantum field theory course of the University of Oxford](../../../split.md)
5. [Quantum field theory course of the University of Oxford](../../../../quantum-field-theory-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
