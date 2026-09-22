<h1 id="10e/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

First prove [continuity](../../../../../../../continuous-function.md) at $b$. Given $\varepsilon>0$, choose $v$ with $\max(c,d-\varepsilon)<v<d$. Surjectivity gives $x_v\in[a,b]$ with $f(x_v)=v$. Strict increase implies $x_v<b$. For $b-(b-x_v)<x\leq b$,

$$
v<f(x)\leq d,\qquad |f(x)-f(b)|<\varepsilon.
$$

Thus $\delta=b-x_v$ proves left [continuity](../../../../../../../continuous-function.md) at $b$. At $a$, choose $c<v<\min(d,c+\varepsilon)$ and use its preimage to prove right [continuity](../../../../../../../continuous-function.md) by the same ordering argument.

For $a<x_0<b$, choose values $v_-,v_+$ in the range such that

$$
\max(c,f(x_0)-\varepsilon)<v_-<f(x_0)<v_+<\min(d,f(x_0)+\varepsilon).
$$

Their preimages satisfy $x_-<x_0<x_+$. If $\delta=\min(x_0-x_-,x_+-x_0)$ and $|x-x_0|<\delta$, strict increase traps $f(x)$ between $v_-$ and $v_+$, so $|f(x)-f(x_0)|<\varepsilon$. Therefore **$f$ is [continuous](../../../../../../../continuous-function.md) on the entire closed interval**. This is [continuity of an increasing interval surjection](../../../../../../../continuity-of-an-increasing-interval-surjection.md): a jump would omit values, contradicting the stated surjectivity.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [10E](../../../10e.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [Ia](../../../../split.md)
6. [2013](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
