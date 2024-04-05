# A Comprehensive Guide to Programming Languages and Their Compilers

<div align=center>

[![TWITTER/X](https://img.shields.io/badge/@naxeion-e05d44?style=for-the-badge&logo=x&color=E42326&logoColor=D9E0EE&labelColor=181b22)](https://x.com/naxeion)
![GitHub commit activity](https://img.shields.io/github/commit-activity/w/naxeion/codeCraftGuide?style=for-the-badge&logo=git&color=E42326&logoColor=D9E0EE&labelColor=181b22)
[![LAST COMMIT](https://img.shields.io/github/last-commit/naxeion/CodeCraftGuide?style=for-the-badge&logo=github&color=E42326&logoColor=D9E0EE&labelColor=181b22)](https://github.com/naxeion/CodeCraftGuide/pulse/monthly)

</div>

The LLVM (Low-Level Virtual Machine) project, a collection of modular and reusable compiler and toolchain technologies, plays a major role in building most programming languages. Integrates with LLVM to generate and optimize code and provide runtime support. LLVM itself is also written primarily in C++.

The project began in 2000 at the University of Illinois by Chris Lattner and Vikram Adve, aiming to provide a modern suite of compiler and toolchain technologies. It has since become foundational in developing various compilers, including those for Swift and Clang.

LLVM is not the only way to build programming languages, but it is one of the popular and powerful tools that can be utilized in this field, there are other methods to building programming languages like Interpreter Engines, Parser Generators, Transpilers, and tools like JVM, CLR, Yacc.

[Swift](#swift) | [Rust](#rust) | [Go](#golang) | [Vala](#vala) | [Lua](#lua)

## Swift

Swift's development began in 2010 and was first introduced by Apple in 2014. Aimed at creating a programming language that was both powerful and user-friendly, Swift sought to overcome the complexities and limitations associated with Objective-C for iOS and macOS development, while Swift's development drew upon ideas from various programming languages. Since its introduction, Swift has seen rapid adoption and has been continuously updated and improved, with contributions from both Apple and the wider developer community.

The Swift compiler, known as the Swift Compiler Frontend, is primarily built using C++. The choice of C++ is due to its performance characteristics and control over system resources, which are crucial for a compiler.

## Rust

Rust's development began in 2006 by Graydon Hoare as a personal project. Officially sponsored by Mozilla in 2009, Rust aimed to create a safer, concurrent, practical language, addressing the pitfalls of C++ used in Mozilla's large, complex systems. The language focused on memory safety without sacrificing performance, a response to the challenges faced in browser development, notably within the Servo project, an experimental browser engine by Mozilla. Rust's first stable release, Rust 1.0, was launched in 2015.

The Rust compiler, known as rustc, was initially written in OCaml. However, as the Rust language matured, it transitioned to a self-hosting architecture, meaning the compiler was rewritten in Rust written in Rust.

Bootstrapping is a process in which a compiler or interpreter for a programming language is written in the same language.

## Golang

Go, also known as Golang, was designed at Google in 2007 by Robert Griesemer, Rob Pike, and Ken Thompson to improve programming productivity in an era of multicore, networked machines, and large codebases. Officially released in 2009, Go aimed to combine the efficiency of compiled languages with the ease of use of interpreted languages. The language addresses critical issues like concurrency, simplicity, and performance, drawing inspiration from C but with improved memory safety and garbage collection.

The initial Go compiler, known as gc, was written in C. It later transitioned to being self-hosting, with the compiler rewritten in Go itself, achieved with Go version 1.5 in 2015.

## Vala

Vala, crafted by Jürg Billeter and Raffaele Sandrini in 2006 and introduced in the same year, aimed to adopt C#'s syntax and semantics without depending on Mono, targeting GNOME's GObject system. Its first version was released to enhance developer productivity through modern language features, while directly compiling to C for performance.

The Vala compiler is written in C and targets the GObject system, aligning with C#'s syntax without requiring Mono, it is similar to the C# syntax. It compiles Vala code into C, remaining non-self-hosting throughout its development.

## Lua

Lua, a lightweight scripting language, was created by Roberto Ierusalimschy, Luiz Henrique de Figueiredo, and Waldemar Celes in 1993 at the Pontifical Catholic University of Rio de Janeiro, Brazil. Designed for embedded use in applications, Lua offers mechanisms for extending programs with custom functions written in Lua or C, without the need for extensive libraries. Its inception was driven by the need for a configurable language for the Petrobras company's data entry forms, aiming to replace data description languages with a more powerful and versatile scripting tool.

Data description languages (DDLs) are specialized languages used for defining data structures and database schemas. They describe the structure of data in a way that allows a database management system (DBMS) or other software to understand how to store, retrieve, and manage data. DDLs typically include commands for creating, altering, and deleting tables, indexes, and other database elements.

The Lua compiler is built in C. This choice creates compatibility with Lua's C API, making it easier to integrate Lua into C applications and extend Lua with C for improved functionality. The development of Lua itself was affected by the limitations faced by its predecessors, SOL and DEL, in particular its lack of control flow structures and the need for more comprehensive programming capabilities within Petrobras' engineering projects.
