<h1 id="b/7/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the auxiliary diffusion $dX_v=\mu X_v\,dv+\sigma X_v\,dW_v$, started at $X_t=x$. Under sufficient regularity and integrability for the [Feynman-Kac formula](../../../../../feynman-kac-formula.md),

$$
\boxed{F(t,x)=\mathbb E\left[
e^{-r(T-t)}\Psi(X_T)+
\int_t^Te^{-r(v-t)}d(v,X_v)\,dv
\,\middle|\,X_t=x\right].}
$$

To verify the signs, apply Itô's formula to $e^{-r(v-t)}F(v,X_v)$. Its drift is $e^{-r(v-t)}(F_t+\mu X_vF_x+\sigma^2X_v^2F_{xx}/2-rF)=-e^{-r(v-t)}d(v,X_v)$. Adding the accumulated source integral makes a martingale; taking expectations through $T$ proves the formula.

Here the auxiliary drift is the printed $\mu$, rather than automatically $r$: this part is a general terminal-value PDE, whose diffusion must match its generator.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [7](../../7.md)
3. [B](../../../b.md)
4. [2008](../../../../2008-split.md)
5. [Past exam of the martingales and financial mathematics course of the University of Oxford](../../../../split.md)
6. [Martingales and financial mathematics course of the University of Oxford](../../../../../martingales-and-financial-mathematics-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
