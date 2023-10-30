<!-- This file is generated from README.org -->

Emacs [tree-sitter](https://tree-sitter.github.io/tree-sitter/) support for the [WebGPU Shading Language (WGSL)](https://gpuweb.github.io/gpuweb/wgsl.html) providing syntax highlighting and navigation.


# Installation

In order to use this mode, you must arrange that the [tree-sitter-wgsl grammar](https://github.com/szebniok/tree-sitter-wgsl/tree/master) is available.


## General

Tree-sitter grammars are unfortunately a separate concern from the emacs support. There is a [section](https://www.masteringemacs.org/article/how-to-get-started-tree-sitter#installing-the-language-grammars) on installing grammars as part of a helpful article on getting started with tree-sitter in emacs that will likely be of use.


## Nix

If you use the [nix](https://nixos.org) package manager, it is available as part of the `treesit-grammars` package that you can include among your other emacs packages with,

    treesit-grammars.with-all-grammars

or you can specify which grammars to include,

    (treesit-grammars.with-grammars (p: [ p.tree-sitter-wgsl ]))

