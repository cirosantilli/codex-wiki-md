<h1 id="7/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

Assume the image of the domain of $f$ lies in the domain where $g$ is [holomorphic](../../../../../holomorphic-function-split.md). The complex [chain rule](../../../../../chain-rule.md) gives

$$
\boxed{(g\circ f)'(z)=g'(f(z))f'(z),}
$$

so the composition is holomorphic, including at points where $f'=0$. Its real part $S(x,y)=s(u(x,y),v(x,y))$ is therefore a [harmonic function](../../../../../harmonic-function.md).

A direct verification uses the [composition of harmonic conjugate pairs](../../../../../composition-of-harmonic-conjugate-pairs.md). The multivariable [chain rule](../../../../../chain-rule.md) gives

$$
\Delta S=s_{uu}|\nabla u|^2+2s_{uv}\nabla u\cdot\nabla v+s_{vv}|\nabla v|^2+s_u\Delta u+s_v\Delta v.
$$

The [Cauchy-Riemann equations](../../../../../cauchy-riemann-equations.md) imply $|\nabla u|^2=|\nabla v|^2$; parts (i) and (ii) remove the last three terms. Since $s$ is harmonic in its own variables,

$$
\boxed{\Delta S=|\nabla u|^2(s_{uu}+s_{vv})=0.}
$$

## ↑ Ancestors (13)

1. [V](../v.md)
2. [7](../../7.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
