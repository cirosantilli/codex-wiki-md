<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The equivalence holds for every lawful [computational monad](../../../../../computational-monad.md) with the semantic equations above. In particular, effects in $e_1$ are neither discarded nor evaluated twice. Fix an initial [semantic environment](../../../../../semantic-environment.md) $\rho$, and write

$$
E=\operatorname{eval}(e_1)\,\rho,\qquad
\rho_v=\operatorname{extend}(\rho,[(x,v)]),\qquad
F(v)=\operatorname{eval}(e_2)\,\rho_v.
$$

Expanding `Let` and `Val` gives

$$
\begin{aligned}
\operatorname{eval}(\mathsf{let\ val}\ x=e_1\ \mathsf{in}\ e_2)\,\rho
&=\bigl(E\triangleright(\lambda v.\,\operatorname{result}(\rho_v))\bigr)
\triangleright(\lambda\rho'.\,\operatorname{eval}(e_2)\,\rho')\\
&=E\triangleright\bigl(\lambda v.\,
\operatorname{result}(\rho_v)\triangleright(\lambda\rho'.\,\operatorname{eval}(e_2)\,\rho')\bigr)\\
&=E\triangleright F.
\end{aligned}
$$

The two steps use [associativity](../../../../../associative-property.md) and left identity from the [monad laws](../../../../../monad-laws.md).

For the application, evaluating the [lambda abstraction](../../../../../lambda-abstraction.md) yields `result c`, where the [programming closure](../../../../../closure-computer-programming.md) $c$ satisfies $\operatorname{apply}(c,[v])=F(v)$. The singleton argument evaluator reduces to

$$
\begin{aligned}
\operatorname{evalArgs}([e_1])\,\rho
&=E\triangleright\bigl(\lambda v.\,
\operatorname{result}([])\triangleright(\lambda vs.\,\operatorname{result}(v:vs))\bigr)\\
&=E\triangleright(\lambda v.\,\operatorname{result}([v])).
\end{aligned}
$$

Use left identity to remove the initial `result c`, then [associativity](../../../../../associative-property.md) and left identity again:

$$
\begin{aligned}
\operatorname{eval}((\mathsf{lambda}(x)\ e_2)\ e_1)\,\rho
&=\bigl(E\triangleright(\lambda v.\,\operatorname{result}([v]))\bigr)
\triangleright(\lambda vs.\,\operatorname{apply}(c,vs))\\
&=E\triangleright\bigl(\lambda v.\,
\operatorname{result}([v])\triangleright(\lambda vs.\,\operatorname{apply}(c,vs))\bigr)\\
&=E\triangleright F.
\end{aligned}
$$

Consequently,

$$
\boxed{\operatorname{eval}(\mathsf{let\ val}\ x=e_1\ \mathsf{in}\ e_2)\,\rho
=\operatorname{eval}((\mathsf{lambda}(x)\ e_2)\ e_1)\,\rho
\quad\text{for every lawful }M.}
$$

The argument relies on the [lambda abstraction](../../../../../lambda-abstraction.md) itself being effect-free, as specified in part (a), and on using the same [semantic environment](../../../../../semantic-environment.md) for $e_1$ on each side. No commutativity of effects is assumed. In particular, the proof applies to [state monads](../../../../../state-monad.md), exceptions and [continuation monads](../../../../../continuation-monad.md), not merely to the [identity monad](../../../../../identity-monad.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Principles of programming languages](../../../principles-of-programming-languages-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
