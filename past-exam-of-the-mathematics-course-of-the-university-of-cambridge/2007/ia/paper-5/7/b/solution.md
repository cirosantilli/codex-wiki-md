<h1 id="7/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A [page table](../../../../../../page-table.md) entry normally supplies validity and access controls. A present/valid bit distinguishes a usable resident translation from an absent or unmapped page; an absent entry forces a [page fault](../../../../../../page-fault.md). A user/supervisor control restricts access to privileged execution or permits user access. Read/write control permits writing or enforces read-only access, protecting code, constants or shared mappings; an attempted forbidden write faults.

Where the architecture supports it, execute permission or a non-executable bit separates instruction fetch from data reads, so writable data need not be executable. Some processors offer separate read, write and execute controls; in the classic 32-bit non-PAE x86 layout matching the stated two-level geometry, there is no independent page execute-disable bit, and a read-only page can still be read and executed. Permissions of every level involved in the page walk must permit the access; the leaf entry cannot override an upper-level restriction.

Accessed/reference and dirty/modified bits are also expected, but they are management information rather than permission bits. They record use and writes for replacement and writeback decisions. Cache-control bits similarly govern memory behavior rather than access authorization. **Validity, privilege and write permission are fundamental; execute permission is architecture-dependent.**

## ↑ Ancestors (11)

1. [B](../b.md)
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
