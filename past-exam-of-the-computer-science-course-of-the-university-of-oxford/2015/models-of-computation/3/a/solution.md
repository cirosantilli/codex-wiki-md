<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Fix a deterministic, single-tape [Turing machine](../../../../../turing-machine.md) with tape cells indexed by the [integers](../../../../../integer-split.md). A precise definition is the [tuple](../../../../../finite-tuple.md)

$$
M=(Q,\Sigma,\Gamma,\delta,q_0,q_{\mathrm{acc}},q_{\mathrm{rej}}),\qquad
\delta:(Q\setminus\{q_{\mathrm{acc}},q_{\mathrm{rej}}\})\times\Gamma
\longrightarrow Q\times\Gamma\times\{L,R\}.
$$

Here $Q$ is a nonempty [finite set](../../../../../finite-set.md) of control states, $\Gamma$ a finite tape [alphabet](../../../../../alphabet.md) with a designated [blank symbol](../../../../../blank-symbol.md) $\square$, $\Sigma\subseteq\Gamma\setminus\{\square\}$ the input [alphabet](../../../../../alphabet.md), $q_0\in Q$ the initial control state, and $q_{\mathrm{acc}},q_{\mathrm{rej}}\in Q$ distinct halting control states. The transition [function](../../../../../function-split.md) is total on the displayed domain. The [Turing machine instruction](../../../../../instruction-of-a-turing-machine.md) $\delta(q,a)=(r,b,D)$ means to write $b$ over the scanned $a$, enter control state $r$, and move the head one cell in direction $D$.

A [Turing machine configuration](../../../../../instantaneous-description-of-a-turing-machine.md) is $(q,\tau,h)$, where $q\in Q$, $h\in\mathbb Z$ is the head position, and $\tau:\mathbb Z\to\Gamma$ is the tape-content [function](../../../../../function-split.md), equal to $\square$ outside a [finite set](../../../../../finite-set.md). Its [next-configuration relation](../../../../../next-configuration-relation.md) is

$$
(q,\tau,h)\vdash_M(r,\tau',h+d)
$$

if $\delta(q,\tau(h))=(r,b,D)$, with $d=-1$ for $D=L$ and $d=1$ for $D=R$, and

$$
\tau'(j)=\begin{cases}b&j=h,\\\tau(j)&j\ne h.\end{cases}
$$

There is no successor to either halting [Turing machine configuration](../../../../../instantaneous-description-of-a-turing-machine.md).

For input $w=a_0\cdots a_{n-1}$, the initial [Turing machine configuration](../../../../../instantaneous-description-of-a-turing-machine.md) is $C_0(w)=(q_0,\tau_w,0)$, where $\tau_w(j)=a_j$ for $0\leq j<n$ and is blank elsewhere. In particular, the initial tape for the [empty word](../../../../../empty-word.md) is entirely blank. The recognized [formal language](../../../../../formal-language.md) is

$$
\boxed{L(M)=\{w\in\Sigma^*:C_0(w)\vdash_M^*(q_{\mathrm{acc}},\tau,h)
\text{ for some }\tau,h\}.}
$$

The relation $\vdash_M^*$ permits any finite number of transitions. An input outside $L(M)$ may reach the rejecting control state or run forever; recognition does not require halting on every input.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Models of computation](../../../models-of-computation-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
