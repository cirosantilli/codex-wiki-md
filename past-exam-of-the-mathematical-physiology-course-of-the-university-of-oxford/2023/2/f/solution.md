<h1 id="2/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

The requested second phase is the second slow recovery phase, beginning after the downward fast jump. Its starting point is $v_3=v_J<0$, fixed by $f(v_J)=f(v_R)$, with the negative root chosen. Along it the same [chain rule](../../../../chain-rule.md) gives

$$
\boxed{h(v)=\frac{f'(v)}{\gamma v-f(v)}
=\frac{-3v^2+2(1+a)v-a}{v[\gamma+a-(1+a)v+v^2]}.}
$$

The approach is to zero from below. Thus, if the printed cutoff $\beta$ is a signed value, it must satisfy $v_J<\beta<0$ and $v_4=\beta$. If $\beta$ denotes a small positive magnitude, the endpoint is instead $v_4=-\beta$. To express both conventions unambiguously, put $b=|\beta|>0$ and write

$$
\boxed{T_2=\int_{v_J}^{-b}h(v)\,dv.}
$$

There is no positive small endpoint on this leading slow branch. A positive cutoff would require a different event or finite-$\varepsilon$ oscillatory recovery.

For bounded negative $v$ and $\gamma\gg1$,

$$
h(v)=\frac1\gamma\left[-3v+2(1+a)-\frac av\right]
+O\!\left(\frac{1+|v|^{-1}}{\gamma^2}\right).
$$

[Integration](../../../../integral-split.md) therefore gives the useful more detailed approximation

$$
T_2=\frac1\gamma\left[
\frac32v_J^2-2(1+a)v_J+a\log\frac{|v_J|}{b}
-2(1+a)b-\frac32b^2\right]
+O\!\left(\frac{1+\log(1/b)}{\gamma^2}\right).
$$

Taking also $b\ll1$, the leading logarithm is

$$
\boxed{T_2\sim\frac a\gamma\log\frac1b.}
$$

Indeed near zero, $f(v)=-av+O(v^2)$ and the slow equation is $\dot v=-(\gamma+a)v/a+O(v^2)$, so at fixed $\gamma$ the exact leading logarithmic coefficient is $a/(\gamma+a)$. Its large-$\gamma$ limit is $a/\gamma$, agreeing with the [integral](../../../../integral-split.md).

The order of approximation matters: first take the [singular limit](../../../../singular-limit.md) at fixed $\gamma$, then the large-$\gamma$ and small-cutoff limits. For simultaneous limits, a sufficient separation near rest is $\varepsilon\gamma\ll a^2$. Otherwise the fast and recovery [time scales](../../../../time-scale.md) merge, and these slow-branch formulas need not describe the late-time motion.

## ↑ Ancestors (12)

1. [F](../f.md)
2. [2](../../2.md)
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
