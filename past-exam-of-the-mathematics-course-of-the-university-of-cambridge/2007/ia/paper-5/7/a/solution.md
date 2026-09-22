<h1 id="7/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A 4096-byte page has a 12-bit offset. Each 1024-entry [page table](../../../../../../page-table.md) needs a 10-bit index, so partition the virtual address as

$$
\boxed{\underbrace{a_{31}\cdots a_{22}}_{\text{directory index: 10 bits}}\quad\underbrace{a_{21}\cdots a_{12}}_{\text{page-table index: 10 bits}}\quad\underbrace{a_{11}\cdots a_0}_{\text{byte offset: 12 bits}}.}
$$

The current process's page-table root points to the first-level directory. The processor first looks for a cached translation of the virtual page in the [translation lookaside buffer](../../../../../../translation-lookaside-buffer.md). On a hit it checks the cached access permissions and combines the physical frame base with the unchanged byte offset.

On a miss, use bits 31--22 to select a directory entry. Its frame address identifies the relevant second-level [page table](../../../../../../page-table.md). Bits 21--12 select the entry giving the data page's physical frame and permissions. With four-byte entries in the usual layout, the entry addresses are directory-base plus four times the first index, and second-level-table-base plus four times the second index. After validity and permission checks, form

$$
\boxed{\text{physical address}=4096\times\text{physical frame number}+(a\bmod4096).}
$$

Populate the translation cache so subsequent accesses avoid the two table reads. A missing or disallowed entry causes a [page fault](../../../../../../page-fault.md). The [operating system](../../../../../../operating-system.md) can supply a valid absent page, update the mapping and restart the instruction, or reject a prohibited access. Table entries and processor state are protected from ordinary user modification. The address-space identifier or root-context rules prevent a cached translation from a different process being used accidentally.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [7](../../7.md)
3. [Paper 5](../../../paper-5-split.md)
4. [Ia](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
