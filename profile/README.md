# The Plainbook Project

A Plainbook is a computational notebook, written in natural language rather than code. 

Normally you would generate a notebook with AI and then keep the code, discarding the natural language that produced it. 
Plainbook keeps the language instead: the code is generated and executed automatically, and can be validated and tested through natural language and data inspection — no coding knowledge required.
This lets you share your data analysis and science with a much wider audience, including people who don't know how to code.

Plainbooks resemble [Jupyter notebooks](https://jupyter.org/), in that they combine instructions and results in a single shareable document. 
They differ in these ways:

* **Linear semantics.** Cells execute strictly in order — the same order in which a human reads the natural-language description of the computation.
* **Dependency tracking.** Code analysis determines what a change actually affects, so only a minimal portion of the Plainbook is regenerated or re-executed.

In these respects, Plainbook is inspired by [Marimo](https://marimo.io/), while being based on natural language. 

The goal of the project is to replicate in natural language what made Jupyter so successful: sharing code and results together, so that any recipient can validate and modify what they receive. 
Recipients can check that the generated code implements the natural-language tasks, and can edit the Plainbook, regenerate the code, and rerun it — just as in Jupyter or Marimo.

## Installation

```bash
pip install plainbook
```

Once installed, you can work on a Plainbook `my_plainbook.plb` via: 

```bash
plainbook my_plainbook.plb
```

## Repositories

* [plainbook](https://github.com/plainbook-ai/plainbook): The main Plainbook code base.
* [snapshot-kernel](https://github.com/plainbook-ai/snapshot-kernel): The kernel implementing state snapshotting on which Plainbook relies for execution.

## Resources

* [Initial Plainbook paper](https://arxiv.org/abs/2607.05717)
* [Pypi package](https://pypi.org/project/plainbook/)
* [Development mailing list](https://groups.google.com/g/plainbook)
