<h1 id="2a/solution">Solution</h1>

↑ **Parent:** [2A](../2a.md)

Set $x=e^z>0$. The [chain rule](../../../../../chain-rule.md) gives $\ddot x=x(\ddot z+\dot z^2)$, so the transformed equation is the forced [harmonic oscillator](../../../../../simple-harmonic-motion.md) $\ddot x+x=-1$, with $x(0)=1$ and $\dot x(0)=V$. Therefore

$$
\boxed{z(t)=\log(2\cos t+V\sin t-1)}.
$$

This real solution is defined only where its [logarithm](../../../../../logarithm.md) has positive argument. Put $R=\sqrt{V^2+4}$ and $\delta=\arctan(V/2)$. Then $x+1=R\cos(t-\delta)$, and the connected interval containing zero is $|t-\delta|<\arccos(1/R)$.

Since $\dot z=\dot x/x$, a [stationary point](../../../../../stationary-point.md) requires $\dot x=0$. The positive branch cannot contain the oscillator minimum $x=-R-1$. It contains the maximum $x=R-1$, attained first at $t=\delta$. Hence

$$
\boxed{z=\log(\sqrt{V^2+4}-1)}.
$$

At the endpoints where $x\downarrow0$, $z$ tends to minus infinity; the oscillator solution cannot be continued through those zeros as a finite real $z$.

## ↑ Ancestors (10)

1. [2A](../2a.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
