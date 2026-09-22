<h1 id="6/d/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For $f'=\Phi(x,f)$, the standard explicit [midpoint method](../../../../../../midpoint-method.md) is

$$
\boxed{\widetilde y_{i+1/2}=y_i+\frac h2\Phi(x_i,y_i),\qquad
y_{i+1}=y_i+h\Phi(x_i+h/2,\widetilde y_{i+1/2}).}
$$

The [implicit midpoint rule](../../../../../../implicit-midpoint-rule.md) instead uses $y_{i+1}=y_i+h\Phi(x_i+h/2,(y_i+y_{i+1})/2)$. When the derivative depends only on $x$, both give $y_{i+1}=y_i+hf'(x_i+h/2)$.

The endpoint-only request in (e) suggests another possible convention: averaging the endpoint slopes, $y_{i+1}=y_i+\tfrac h2[\Phi(x_i,y_i)+\Phi(x_{i+1},y_{i+1})]$. This is the [trapezoidal rule](../../../../../../trapezoidal-rule.md), and generally differs from the [implicit midpoint rule](../../../../../../implicit-midpoint-rule.md). A further use of “midpoint” is the two-step [explicit midpoint linear multistep method](../../../../../../explicit-midpoint-linear-multistep-method.md), $y_{i+1}=y_{i-1}+2h\Phi(x_i,y_i)$, which needs a second starting value. The printed question supplies no convention to distinguish these meanings; (e) spells out the resulting alternatives.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [D](../../d.md)
3. [6](../../../6.md)
4. [Discrete mathematics, continuous mathematics and probability](../../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
5. [2016](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
