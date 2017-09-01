---
layout: default
---

# Revisiting Visitors for Modular Extension of DSMLs

## Overview

*Revisitor* is a new language implementation pattern that enables independent extensibility of the syntax and the semantics of metamodel-based xDSMLs with incremental compilation and without anticipation.

On top of the *Revisitor* pattern, we introduce ALE (Action Language for Ecore): a high-level semantics specification language that supports modular extension of both syntax and semantics where the *Revisitor* pattern ensures separate compilation of language modules.

ALE is tightly integrated with the [Eclipse Modeling Framework](https://www.eclipse.org/modeling/emf/) (EMF) and rely on the Ecore meta-language for the definition of the abstract syntax of the xDSMLs. Operational semantics is defined using ALE and the *open class* mechanism. ALE is bundled as a set of Eclipse plug-ins. Please refer to the [Github repository](https://github.com/manuelleduc/ale-compiler/) for more information.

## MODELS'17

For more information on ALE and the *Revisitor* pattern, please refer to [our MODELS'17 paper](https://hal.inria.fr/hal-01568169).

> Executable Domain-Specific Modeling Languages (xDSMLs) are typically defined by metamodels that specify their abstract syntax, and model interpreters or compilers that define their execution semantics.
To face the proliferation of xDSMLs in many domains, it is important to provide language engineering facilities for opportunistic reuse, extension, and customization of existing xDSMLs to ease the definition of new ones.
>Current approaches to language reuse either require to anticipate reuse, make use of advanced features that are not widely available in programming languages, or are not directly applicable to metamodel-based xDSMLs.
>In this paper, we propose a new language implementation pattern that enables independent extensibility of the syntax and semantics of metamodel-based xDSMLs with incremental compilation and without anticipation.
>We seamlessly implement our approach alongside the compilation chain of the Eclipse Modeling Framework, thereby demonstrating that it is directly and broadly applicable in various modeling environments.
>We show how it can be employed to incrementally extend both the syntax and semantics of the fUML language without requiring anticipation or re-compilation of existing code, and with acceptable performance penalty compared to classical handmade visitors.


## Examples and benchmarks

All examples of the paper as well as the implementations used in the benchmarks are available on [a dedicated Github repository](https://github.com/manuelleduc/ale-compiler-benchmarks).

