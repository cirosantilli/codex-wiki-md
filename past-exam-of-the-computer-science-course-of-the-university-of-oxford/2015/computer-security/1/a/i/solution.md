<h1 id="1/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [Bell-LaPadula model](../../../../../../bell-lapadula-model.md) protects [information confidentiality](../../../../../../information-confidentiality.md) by controlling information flow between security levels. Its [simple security property](../../../../../../simple-security-property.md) says that a subject may read only objects whose classification does not exceed its maximum clearance:

$$
f_O(o)\le f_S(s).
$$

Thus a user cleared for confidential material cannot directly read a secret file. A [readwrite](../../../../../../readwrite.md) permission includes reading and must satisfy the same restriction. This is an [access control](../../../../../../access-control.md) rule about who can learn existing contents; it says nothing by itself about where a cleared subject can subsequently copy them.

$$
\boxed{\text{The ss-property enforces confidentiality: no reading above maximum clearance.}}
$$

## ↑ Ancestors (12)

1. [I](../i.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [Computer security](../../../../computer-security-split.md)
5. [2015](../../../../split.md)
6. [Past exam of the computer science course of the University of Oxford](../../../../../split.md)
7. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
