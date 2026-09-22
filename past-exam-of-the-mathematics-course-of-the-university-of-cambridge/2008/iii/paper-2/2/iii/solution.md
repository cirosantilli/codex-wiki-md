<h1 id="2/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The [halting problem](../../../../../../halting-problem.md) asks whether program $e$ halts on input $x$, given effective codes for both. Suppose a total decision algorithm $H(e,x)$ returned one exactly when that computation halts. Construct a program $D$ which, on input $e$, computes $H(e,e)$ and then loops forever if the answer is one, but halts if it is zero. Let $d$ be the code of $D$. If $H(d,d)=1$, the specification of $D$ makes it diverge, while if $H(d,d)=0$ the same specification makes it halt. Both alternatives contradict correctness. Therefore **the halting problem is $\boxed{\text{undecidable}}$.** This is a [diagonal argument](../../../../../../diagonal-argument.md), not merely the observation that individual simulations can run forever.

Let $K=\{e:\text{program }e\text{ halts on input }e\}$. Simulating the specified program semidecides membership, or [dovetailing](../../../../../../dovetailing.md) all simulations enumerates $K$, so $K$ is a [recursively enumerable set](../../../../../../recursively-enumerable-set.md). The same diagonal program rules out a total decision algorithm for $K$. Thus $\boxed{K\text{ is recursively enumerable but not recursive}}$. Encoding a pair $(e,x)$ also gives an enumerable nonrecursive set of all halting program-input pairs.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [2](../../2.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
