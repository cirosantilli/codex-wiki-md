<h1 id="10/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

A fully [synchronous sequential circuit](../../../../../../synchronous-sequential-circuit.md) has all its state stored in edge-triggered elements driven by a common [clock signal](../../../../../../clock-signal.md), with combinational logic computing the next state from the current state and inputs. State updates occur together at the designated [clock edges](../../../../../../clock-edge.md), rather than letting one register output serve as another register's ripple clock. Its ideal equations are

$$
\boxed{s_{k+1}=F(s_k,u_k),\qquad z_k=G(s_k,u_k).}
$$

For a [Moore machine](../../../../../../moore-machine.md) the output [function](../../../../../../function-split.md) depends only on the state, $z_k=G(s_k)$. Physical design must leave enough time for register-to-register combinational paths and satisfy [setup time](../../../../../../setup-time.md) and [hold time](../../../../../../hold-time.md) at every receiving storage element.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [10](../../../10.md)
4. [Functional programming, data structures and algorithms, procedural programming, and digital hardware](../../../../functional-programming-data-structures-and-algorithms-procedural-programming-and-digital-hardware-split.md)
5. [2003](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
