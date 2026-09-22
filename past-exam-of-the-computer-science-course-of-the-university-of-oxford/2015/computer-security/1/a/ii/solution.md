<h1 id="1/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [Bell-LaPadula star property](../../../../../../bell-lapadula-star-property.md) restricts information flow using the subject's current level. With the paper's distinction between blind writing and reading, its usual current-level formulation is

| Access | Required comparison |
| --- | --- |
| Read | $f_O(o)\le f_C(s)$ |
| Blind write | $f_C(s)\le f_O(o)$ |
| Readwrite | $f_C(s)=f_O(o)$ |

Here $f_C(s)\le f_S(s)$ also holds. The first row means that reading above the current level is forbidden; the second is the familiar prohibition on writing down. Their conjunction gives the third row. Blind writing upwards is allowed because it need not disclose the higher file's contents to the writer.

For example, a subject operating at secret level cannot copy a secret file into a public file, even though its clearance would permit reading both files. More generally, any simultaneously readable object must be at most as highly classified as any writable object. A subject must not evade the rule by retaining secret information and then lowering its current level: level-changing transitions need their own safe treatment of retained information and open accesses.

$$
\boxed{\text{Read at or below the current level; write at or above it.}}
$$

## ↑ Ancestors (12)

1. [Ii](../ii.md)
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
