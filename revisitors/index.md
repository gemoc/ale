---
layout: default
---

# Revisiting Visitors for Modular Extension of DSMLs (Models'17)

> Executable Domain-Specific Modeling Languages
(xDSMLs) are typically defined by metamodels that specify their
abstract syntax, and model interpreters or compilers that define
their execution semantics. To face the proliferation of xDSMLs in
many domains, it is important to provide language engineering
facilities for opportunistic reuse, extension, and customization
of existing xDSMLs to ease the definition of new ones. Current
approaches to language reuse either require to anticipate reuse,
make use of advanced features that are not widely available
in programming languages, or are not directly applicable to
metamodel-based xDSMLs. In this paper, we propose a new
language implementation pattern that enables independent ex-
tensibility of the syntax and semantics of metamodel-based
xDSMLs with incremental compilation and without anticipation.
We seamlessly implement our approach alongside the compilation
chain of the Eclipse Modeling Framework, thereby demonstrating
that it is directly and broadly applicable in many modeling
environments. We show how it can be employed to incrementally
extend both the syntax and semantics of the fUML language
without requiring anticipation or re-compilation of existing code,
and with no significant runtime penalty compared to classical
handmade visitors.
