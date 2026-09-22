<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Allow clean workspace bits, as in standard [reversible computation](../../../../reversible-computation.md). [Boolean algebra](../../../../boolean-algebra.md) expresses any [Boolean function](../../../../boolean-function.md) as XORs of ANDs and constants. A [Toffoli gate](../../../../toffoli-gate.md) maps $(a,b,c)$ to $(a,b,c\oplus ab)$, so an initially zero target computes an [AND](../../../../logical-conjunction.md) without erasing the inputs. A [CNOT gate](../../../../controlled-not-gate.md) accumulates XORs, and a [NOT gate](../../../../pauli-x-gate.md) supplies complemented bits or constants. Intermediate products can be computed into workspace, XORed into an output, and then [uncomputed](../../../../uncomputation.md) by reversing the workspace computation. This realizes the reversible embedding $(x,y)\mapsto(x,y\oplus f(x))$ for any [Boolean function](../../../../boolean-function.md) and, with reversible clean-up, universal reversible classical computation.

The [Fredkin](../../../../fredkin-gate.md) transformation has control $a$ and targets $b,c$. A network of three gates, shown in [i](../../4/b/i.md), is

$$
\boxed{\operatorname{CNOT}_{b\to c}\ ;\quad
\operatorname{Toffoli}_{a,c\to b}\ ;\quad
\operatorname{CNOT}_{b\to c},}
$$

where the sequence is executed left to right. After the first gate $c_1=c\oplus b$; after the second $b_1=b\oplus a(c\oplus b)$; and the last gives $c_2=c\oplus b\oplus b_1$. If $a=0$, $(b_1,c_2)=(b,c)$; if $a=1$, $(b_1,c_2)=(c,b)$. Thus the circuit is exactly a [Fredkin gate](../../../../fredkin-gate.md).

The workspace qualification matters for the unrestricted universality claim. On four or more wires, every embedded NOT, [CNOT](../../../../controlled-not-gate.md) and [Toffoli gate](../../../../toffoli-gate.md) is an even permutation of all computational states. Without [ancillary wires](../../../../quantum-ancilla.md) they cannot implement, for example, a permutation swapping just $0000$ and $0001$ while fixing the other four-bit strings. Clean [ancillas](../../../../quantum-ancilla.md) remove this obstruction on the designated input subspace.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [5](../../5.md)
3. [2019](../../../2019-split.md)
4. [Past exam of the laser science and quantum information processing course of the University of Oxford](../../../split.md)
5. [Laser science and quantum information processing course of the University of Oxford](../../../../laser-science-and-quantum-information-processing-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
