<h1 id="2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Suppose the operands are initially stable and written in [CSP external choice](../../../../../csp-external-choice.md) normal form,

$$
P=\mathop{\square}_{a\in B}a\to P_a,\qquad Q=\mathop{\square}_{a\in C}a\to Q_a.
$$

The [CSP step law](../../../../../csp-step-law.md) is

$$
\boxed{\begin{aligned}
J_A(P,Q)
&=\mathop{\square}_{a\in B\setminus A}a\to J_A(P_a,Q)\\
&\quad\mathbin\square\mathop{\square}_{a\in C\setminus A}a\to Q_a\\
&\quad\mathbin\square\mathop{\square}_{a\in B\cap C\cap A}a\to J_A(P_a,Q_a).
\end{aligned}}
$$

An empty indexed [CSP external choice](../../../../../csp-external-choice.md) denotes $\mathrm{STOP}$. A label appearing in both of the first two lines must retain both continuations: after that common label the result is the [CSP internal choice](../../../../../csp-internal-choice.md) between the continuations. A label in $A$ appears only in the third line and only if both operands offer it. These are exactly the three visible-transition rules from part (d); the two [CSP internal action](../../../../../csp-internal-action.md) rules handle operands that are not initially stable.

As a check, for the paper's example the initial shared $a$ leads to $J_{\{a\}}(b\to\mathrm{STOP},c\to\mathrm{STOP})$. Its expansion is

$$
b\to J_{\{a\}}(\mathrm{STOP},c\to\mathrm{STOP})\mathbin\square c\to\mathrm{STOP}
=b\to c\to\mathrm{STOP}\mathbin\square c\to\mathrm{STOP},
$$

which recovers the displayed example after prefixing by $a$.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [2](../../2.md)
3. [Concurrency](../../../concurrency-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
