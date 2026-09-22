<h1 id="f/1/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Applying the [chain rule](../../../../../chain-rule.md) to both inverse identities gives

$$
\boxed{D(f^{-1})(f(a))=[Df(a)]^{-1}.}
$$

For the unnumbered calculation, the requested point is $f(c,c)$. The Jacobian there is

$$
Df(c,c)=\begin{pmatrix}e^c&e^c\\e^c&-e^{-c}\end{pmatrix},\qquad\det Df(c,c)=-(e^{2c}+1)\ne0.
$$

To apply its inverse to $(1/2,1/2)$, solve $e^c(v_1+v_2)=1/2$, $e^cv_1-e^{-c}v_2=1/2$. Subtraction gives $v_2=0$, and hence

$$
\boxed{D_{(1/2,1/2)}f^{-1}(2e^c,2\cosh c)=\left(\frac{e^{-c}}2,0\right).}
$$

For precision, the displayed example maps bijectively onto $V=\{(s,t):s>0,t>0,st>1\}$, rather than the entire positive quadrant. Indeed writing $q=e^x$, the equations are $(s-q)(t-q)=1$ with $0<q<\min(s,t)$. This left side decreases continuously from $st$ to zero, giving exactly one $q$ if and only if $st>1$, after which $e^y=s-q$ is unique. Its Jacobian never vanishes, so the inverse is differentiable on $V$. The requested point lies in $V$, making the calculation well-defined.

## ↑ Ancestors (13)

1. [Iv](../iv.md)
2. [1](../../1.md)
3. [F](../../../f.md)
4. [2005](../../../../2005-split.md)
5. [Past exam of the options I course of the University of Oxford](../../../../split.md)
6. [Options I course of the University of Oxford](../../../../../options-i-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
