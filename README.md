# Data Structure Optimization for Functional Programs

## Abstract

The purpose of this work is to develop techniques to allow
for executing programs written in functional style effectively.
The work consists of two parts. The first one shows some classic
techniques for transforming functional programs into imperative form,
as well as some basic methods of proving statements about program
properties. In the second part, a method for transforming a certain
class of programs operating on lists into equivalent programs
operating on arrays is proposed. Furthermore, the conditions allowing
to transform a functional implementation of quick sort algorithm
into an optimal imperative form are analyzed.

All source programs and transformations are expressed using the
purely functional subset of the algorithmic language Scheme, as
described in chapter 2. The target computation model is a variant
of the RAM machine, whose model and instruction set were described
in depth in chapter 3, including an implementation, which uses
some imperative features of the Scheme programming language.

In chapter 4 some classic techniques of transforming programs expressed
in the previously described subset of Scheme into sequences of instructions
for the RAM machine are presented; in particular, the conversion to
Continuation-Passing Style and Tail-Call Optimization are described.

Chapter 5 describes a simplified variant of the Boyer-Moore system,
including a full list of axioms used for proving theorems about programs
expressed in the previously described subset of the Scheme programming
language. Unlike the original Boyer-Moore system, however, the system
elaborated in our work is incapable of proving theorems on its own,
and can only serve as a proof-checker for the proofs provided by its
user.

In chapter 6 an original method for converting functional programs
into forms receiving and passing arrays is developed. The source
language is the purely functional subset of Scheme described in chapter
2, and the target language is the full Scheme language, including its
imperative features. The proposed conversion method is only sketchy
and certainly requires elaboration.

Chapter 7 deals with automatic conversion of a functional variant
of the quick sort algorithm into an imperative form, although it
fails to present a working conversion algorithm.

## Keywords

data structure, program transformation, compiler, theorem prover,
functional programming
