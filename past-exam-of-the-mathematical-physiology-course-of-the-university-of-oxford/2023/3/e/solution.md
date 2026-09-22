<h1 id="3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Differentiate the identity $f(u,g(u))=0$ using the [chain rule](../../../../chain-rule.md):

$$
f_u+f_vg'(u)=0,\qquad f_u=-f_vg'(u).
$$

Substitution into the [trace](../../../../matrix-trace.md) gives

$$
\operatorname{tr}J=-1+\frac{f_v}{\varepsilon}\bigl(1+\gamma g'(\mu)\bigr).
$$

Because $f_v<0$, the exact instability condition is

$$
\boxed{1+\gamma g'(\mu)<\frac\varepsilon{f_v},\qquad
g'(\mu)<-\frac1\gamma+\frac{\varepsilon}{\gamma f_v}.}
$$

For fixed $\delta>0$ and fixed [equilibrium](../../../../equilibrium-point-of-a-dynamical-system.md) location, the correction tends to zero with $\varepsilon$. To leading order this is

$$
\boxed{g'(\mu)<-1/\gamma.}
$$

Thus instability requires the descending [nullcline](../../../../nullcline.md) to be steeper than a line of slope $-1/\gamma$. The sign of the finite-$\varepsilon$ correction makes the exact unstable interval slightly smaller. Since $\delta=0.001$ can make $|f_v|$ small, the approximation quantitatively requires $\varepsilon/|f_v|\ll1$ at the point in question; merely comparing $\varepsilon$ with one can be insufficient.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [3](../../3.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the mathematical physiology course of the University of Oxford](../../../split.md)
5. [Mathematical physiology course of the University of Oxford](../../../../mathematical-physiology-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
