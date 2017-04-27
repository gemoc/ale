---
layout: default
---

# Revisiting Visitors for Modular Extension of DSMLs

## Overview

The *Revisitors* are a new language implementation pattern that enables independent
extensibility of the syntax and the semantics of metamodel-based xDSMLs with
incremental compilation and without anticipation. This pattern is inspured by
the [Object Algebra](https://dl.acm.org/citation.cfm?id=2367167) design pattern.

On top of the *Revisitors* we introduce *ALE*, a high-level specification language supporting modular extension of both syntax and semantics where the *Revisitor* pattern ensures separate compilation of language modules.

*Ale* is tightly integrated with the [Eclipse Modeling Framework](https://www.eclipse.org/modeling/emf/) (EMF) and rely on the Ecore meta-language for the definition of the absatract syntax of the xDSMLs. Operation semantics is defined using *Ale* using *open class* definitions. *Ale* is bundle as a set of Eclipse plug-ins. Please referer to the [installation instructions](https://github.com/manuelleduc/ale-compiler/blob/master/Readme.md#installation) for more information.

## Models'17

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

## Examples and benchmarks

All the examples of the paper as well as the implementations used in the benchmarks are available at [manuelleduc/ale-compiler-benchmarks](https://github.com/manuelleduc/ale-compiler-benchmarks).
