<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

At fixed positive $x$ the leading [outer expansion](../../../../../../outer-expansion.md) satisfies $z_0'+z_0=e^{-x}/x$. Integrating and imposing the value at one yields

$$
z_0=e^{-x}(1+\log x).
$$

It diverges negatively at zero, and the neglected nonlinear shift in the [derivative](../../../../../../derivative.md) coefficient becomes important when $x\sim\varepsilon|\log x|$. Thus the relevant [logarithmically enhanced nonlinear boundary layer](../../../../../../logarithmically-enhanced-nonlinear-boundary-layer.md) is larger than a plain $O(\varepsilon)$ layer. Write $L=\log(1/\varepsilon)$, $x=\varepsilon L X$ and

$$
z=-L+\log L+1+Z(X)+o(1).
$$

For fixed $X$, the leading inner equation is $(X+1)Z_X=1$. Matching to the outer logarithm, for which $Z\sim\log X$, sets the integration constant and gives

$$
Z=\log(1+X),\qquad z(0)=-L+\log L+1+o(1).
$$

In particular the exact equation at zero is $-\varepsilon z(0)z'(0)=1$, so

$$
\boxed{z'(0)\sim\frac1{\varepsilon\log(1/\varepsilon)}>0}.
$$

An implicit inner form also checks the matching constants. With $x=\varepsilon\xi$, retain $z$ without assigning it a bounded size. The leading equation is $(\xi-z)z_\xi=1$. Inverting it gives $d\xi/dz-\xi=-z$, hence

$$
\xi=z+1+B e^z.
$$

Its large-$\xi$ match to $z\sim1+\log\varepsilon+\log\xi$ fixes $B\sim e^{-1}/\varepsilon$. Taking that matched leading value at zero gives

$$
z(0)\simeq-1-W_0(e^{-2}/\varepsilon),\qquad
z'(0)\simeq\frac1{\varepsilon[1+W_0(e^{-2}/\varepsilon)]},
$$

where $W_0$ is the positive real branch of the [Lambert W function](../../../../../../lambert-w-function.md). Its large-argument expansion reproduces the logarithm and log-log terms above. This refinement is a matched approximation, not an exact solution of the full equation; the leading slope conclusion follows directly from the first inner scaling and the exact endpoint identity.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 74](../../../paper-74-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
