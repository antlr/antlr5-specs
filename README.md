# antlr5-specs

This repo is the place where we discuss specs for antlr5.
It's a private repo for now because we want to be effective (large groups tend to introduce inertia).

Antlr5 is the next major version of Antlr.

It's driven by several business goals:
 - browser first: the move to the web hasn't slowed down. Having a fast parser in a browser without the need for a backend is needed.
 - LSP integration: we currently only properly support 1 IDE. It slows down adoption of Antlr. Using LSP, all IDEs will support Antlr, making it easier to adopt.
 - Unified runtime: thanks to WebAssembly, we can have a single runtime for all mainstream targets, improving consistency whilst reducing maintenance
 - Targets as add-ons: we are not able to support our existing targets, and creating one outside Antlr is a big piece of work. We will focus on a small set of core targets, and let developers easily create new lightweight targets.

It's also the opportunity to indroduce new features:
  - templates for production code
  - includes in lexer grammars
  - built-in macros for common patterns
  - token categories
  - contextual tokens
  - ...

Antlr5 relies on WebAssembly, which is still bleeding edge, notably for required features such as GC.
We believe it will take many months before it is mature enough for production.
We're using this time and this space to clarify how Antlr5 will look like, and to make informed technical decisions.

All the efforts happen in [this repo's GitHub discussions](https://github.com/antlr/antlr5-specs/discussions).
