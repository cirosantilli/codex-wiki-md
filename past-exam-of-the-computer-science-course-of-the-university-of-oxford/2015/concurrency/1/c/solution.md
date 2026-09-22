<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $X=P\ {}_{\{a,b,d\}}\Vert_{\{a,b,c\}}\ Q$. In this [CSP alphabetized parallel composition](../../../../../csp-alphabetized-parallel-composition.md), $a,b$ require both participants, $d$ belongs only to the left participant and $c$ only to the right participant. Expand the reachable states using [CSP prefixing](../../../../../csp-prefixing.md) and [CSP external choice](../../../../../csp-external-choice.md):

$$
\begin{aligned}
X&=a\to Y,\\
Y&=b\to Z\mathbin\square d\to W,\\
W&=b\to Z,\\
Z&=c\to X.
\end{aligned}
$$

For example, after the synchronized $b$, the left participant is back at $P$ but the right participant is at $c\to Q$. The left participant's proposed $a$ is blocked until the right participant has performed $c$. Similarly, after $a,d$, only the synchronized $b$ is possible. Thus there is no extra interleaving to include.

Eliminating $Y,W,Z$ gives the guarded equation

$$
X=a\to\bigl(b\to c\to X\mathbin\square d\to b\to c\to X\bigr).
$$

Consequently choose the sequential [CSP process](../../../../../csp-process.md)

$$
\boxed{R=a\to\bigl(b\to c\to R\mathbin\square d\to b\to c\to R\bigr).}
$$

The [unique fixed point principle](../../../../../unique-fixed-point-principle.md) first establishes $R=X$.

Now let $E=X\mathbin\Theta_{\{c\}}X$. The [CSP exception](../../../../../csp-exception.md) operator follows its left operand until that operand performs $c$, includes this $c$ in the visible behaviour, and then switches to its right operand. Applying its [CSP step law](../../../../../csp-step-law.md) to the four-state expansion yields

$$
E=a\to\bigl(b\to c\to X\mathbin\square d\to b\to c\to X\bigr)=X.
$$

The switch occurs exactly where the ordinary execution already returns to $X$. Therefore $E=X=R$. The answer uses neither a [CSP exception](../../../../../csp-exception.md) operator nor a [CSP parallel composition](../../../../../csp-parallel-composition.md) operator, and the argument gives equality in all three standard [CSP semantic models](../../../../../csp-semantic-model.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Concurrency](../../../concurrency-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
