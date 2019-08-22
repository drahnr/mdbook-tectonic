# mdbook-latex

[![crates badge][crates-badge]][crates.io]
[![docs badge][docs-badge]][docs]

[crates.io]: https://crates.io/crates/mdbook-latex
[crates-badge]: https://img.shields.io/badge/crates.io-v0.1.0-orange.svg?longCache=true

[docs]: https://docs.rs/crate/mdbook-latex/0.1.0
[docs-badge]: https://docs.rs/mdbook-latex/badge.svg

An [mdbook](https://github.com/rust-lang-nursery/mdBook) backend for generating LaTeX and PDF documents.

> **Warning**: Not yet stable — may eat, shred, and atomize your laundry! See the [**Are We Stable Yet?**](#are-we-stable-yet%3F) section for a roadmap to the production release.

## Status of Rust Bookshelf

- ✅ compiles successfully
- 🍊 compiles but with warnings/errors
- ❌ compilation fails/not yet attempted

| Compiles? | Generated PDF                          | Generated LaTeX                 | Source                     | Online Version            |
| --------- | ---------------------------------      | -----------------------         | ----------------------     | ---------------------     |
| ❌        | [~~Cargo Book~~][cargo-pdf]            | [~~LaTeX~~][cargo-latex]        | [Source][cargo-src]        | [HTML][cargo-html]        |
| ❌        | [~~Edition Guide~~][edition-pdf]       | [~~LaTeX~~][edition-latex]      | [Source][edition-src]      | [HTML][edition-html]      |
| ❌        | [~~Embedded Rust Book~~][embedded-pdf] | [~~LaTeX~~][embedded-latex]     | [Source][embedded-src]     | [HTML][embedded-html]     |
| ❌        | [~~Mdbook User Guide~~][mdbook-pdf]    | [~~LaTeX~~][mdbook-latex]       | [Source][mdbook-src]       | [HTML][mdbook-html]       |
| ❌        | [~~Rust Reference~~][reference-pdf]    | [~~LaTeX~~][reference-latex]    | [Source][reference-src]    | [HTML][reference-html]    |
| ❌        | [~~Rust By Example~~][example-pdf]     | [~~LaTeX~~][example-latex]      | [Source][example-src]      | [HTML][example-html]      |
| 🍊        | [Rust Programming Language][rust-pdf]  | [LaTeX][rust-latex]             | [Source][rust-src]         | [HTML][rust-html]         |
| ❌        | [~~Rustc Book~~][rustc-pdf]            | [~~LaTeX~~][rustc-latex]        | [Source][rustc-src]        | [HTML][rustc-html]        |
| ❌        | [~~Rustdoc Book~~][rustdoc-pdf]        | [~~LaTeX~~][rustdoc-latex]      | [Source][rustdoc-src]      | [HTML][rustdoc-html]      |
| ❌        | [~~Rustonomicon~~][rustonomicon-pdf]   | [~~LaTeX~~][rustonomicon-latex] | [Source][rustonomicon-src] | [HTML][rustonomicon-html] |
| ❌        | [~~Unstable Book~~][unstable-pdf]      | [~~LaTeX~~][unstable-latex]     | [Source][unstable-src]     | [HTML][unstable-html]     |

[rust-pdf]: https://github.com/lbeckman314/mdbook-latex/releases/download/v0.1.1/The.Rust.Programming.Language.pdf
[rust-latex]: https://github.com/lbeckman314/mdbook-latex/releases/download/v0.1.1/The.Rust.Programming.Language.tex
[rust-src]: https://github.com/rust-lang/book
[rust-html]: https://doc.rust-lang.org/book/

[mdbook-pdf]: https://github.com/lbeckman314/mdbook-latex/releases
[mdbook-latex]: https://github.com/lbeckman314/mdbook-latex/releases
[mdbook-src]: https://github.com/rust-lang-nursery/mdBook/tree/master/book-example
[mdbook-html]: https://rust-lang-nursery.github.io/mdBook/

[example-pdf]: https://github.com/lbeckman314/mdbook-latex/releases
[example-latex]: https://github.com/lbeckman314/mdbook-latex/releases
[example-src]: https://github.com/rust-lang/rust-by-example
[example-html]: https://doc.rust-lang.org/stable/rust-by-example/

[edition-pdf]: https://github.com/lbeckman314/mdbook-latex/releases
[edition-latex]: https://github.com/lbeckman314/mdbook-latex/releases
[edition-src]: https://github.com/rust-lang-nursery/edition-guide
[edition-html]: https://doc.rust-lang.org/edition-guide/index.html

[rustc-pdf]: https://github.com/lbeckman314/mdbook-latex/releases
[rustc-latex]: https://github.com/lbeckman314/mdbook-latex/releases
[rustc-src]: https://github.com/rust-lang/rustc-guide
[rustc-html]: https://doc.rust-lang.org/rustc/index.html

[cargo-pdf]: https://github.com/lbeckman314/mdbook-latex/releases
[cargo-latex]: https://github.com/lbeckman314/mdbook-latex/releases
[cargo-src]: https://github.com/rust-lang/cargo/tree/master/src/doc
[cargo-html]: https://doc.rust-lang.org/cargo/index.html

[rustdoc-pdf]: https://github.com/lbeckman314/mdbook-latex/releases
[rustdoc-latex]: https://github.com/lbeckman314/mdbook-latex/releases
[rustdoc-src]: https://github.com/rust-lang/rust/tree/master/src/doc/rustdoc
[rustdoc-html]: https://doc.rust-lang.org/rustdoc/index.html

[reference-pdf]: https://github.com/lbeckman314/mdbook-latex/releases
[reference-latex]: https://github.com/lbeckman314/mdbook-latex/releases
[reference-src]: https://github.com/rust-lang-nursery/reference
[reference-html]: https://doc.rust-lang.org/reference/index.html

[rustonomicon-pdf]: https://github.com/lbeckman314/mdbook-latex/releases
[rustonomicon-latex]: https://github.com/lbeckman314/mdbook-latex/releases
[rustonomicon-src]: https://github.com/rust-lang-nursery/nomicon
[rustonomicon-html]: https://doc.rust-lang.org/nomicon/index.html

[unstable-pdf]: https://github.com/lbeckman314/mdbook-latex/releases
[unstable-latex]: https://github.com/lbeckman314/mdbook-latex/releases
[unstable-src]: https://github.com/rust-lang/rust/tree/master/src/doc/unstable-book
[unstable-html]: https://doc.rust-lang.org/unstable-book/index.html

[embedded-pdf]: https://github.com/lbeckman314/mdbook-latex/releases
[embedded-latex]: https://github.com/lbeckman314/mdbook-latex/releases
[embedded-src]: https://github.com/rust-embedded/book
[embedded-html]: https://rust-embedded.github.io/book/

## Installation

First, install the following two programs:

- [Rust](https://www.rust-lang.org/)
- [mdbook](https://github.com/rust-lang-nursery/mdBook)

Then, to install `mdbook-latex`, enter the following in a shell:

```sh
cargo install mdbook-latex
```

Finally, add the following `toml` configuration to `book.toml`.

```toml
[output.latex]
latex = true
pdf = true
```

The next `mdbook build` command will produce LaTeX and PDF files in the `book/latex/` directory.

## Uninstallation

To uninstall `mdbook-latex`, enter the following in a shell:

```sh
cargo uninstall mdbook-latex
```

Then delete the `[output.latex]` configuration in `book.toml`:

```diff
- [output.latex]
- latex = true
- pdf = true
```

## Primary Dependencies

`mdbook-latex` is built upon some really wonderful projects, including:

- [pulldown-cmark](https://github.com/raphlinus/pulldown-cmark): Parses the markdown source AST.
- [Tectonic](https://tectonic-typesetting.github.io/en-US/): Creates the final PDF file from the transformed LaTeX code.
- [md2tex](https://github.com/lbeckman314/md2tex): Transforms the markdown source to LaTeX. This is a fork of [md2pdf](https://gitea.tforgione.fr/tforgione/md2pdf/), a great utility for converting markdown code to LaTeX and PDF's.  I hope to eventually propose some of the updates back upstream. `md2tex` and `mdbook-latex` are developed in tandem, but are meant to be independent programs. Therefore, if one wishes to use an alternative markdown-to-tex conveter, they should be able to plug it in to `mdbook-latex` with ease.

## How's it Work?

Broadly speaking, there are three steps, or "transformations", from `mdbook` source to PDF output:

1) **mdbook source to JSON-organized markdown** (`mdbook-latex`): retreives the JSON formatted data from `mdbook`. Calls `md2tex` and `tectonic` for LaTeX and PDF generation, respectively.
2) **markdown to LaTeX** (`md2tex`): converts markdown input to LaTeX output.
3) **LaTeX to PDF** (`tectonic`): creates PDF document from LaTeX input.

## Contributing

Pull requests, forks, and plain old copy-pasting are actively encouraged! Also, I am relatively new to Rust (and programming in general) so recommendations or advice in general is always appreciated.

### I found a problem. Should I create an issue with `mdbook-latex` or `md2tex`?

Either one. `mdbook-latex` can be thought of as a frontend for the LaTeX generation done by `md2tex`. So if there is a LaTeX error, you may favor creating an issue with `md2tex`. Otherwise, creating an issue with `mdbook-latex` is a good bet. But any issue is a good issue, so don't worry if it's in the "right" repository or not, I should be able to see it regardless!

## Are We Stable Yet?

Below is a list of features I am currently working on (loosly in "top-down" direction).

- [ ] Add support for equation delimiters "\( x^2 \)" "\[ x^2 \]". 
- [ ] Allow SVG images (convert to PNG for LaTeX).
    - [x] Configure [resvg](https://github.com/RazrFalcon/resvg) library to convert SVG's to PNG.
    - [ ] Save SVG's in `book/latex` directory to keep `src` clean.
- [ ] Add CI/CD pipeline ([travis](https://travis-ci.org/))
- [ ] Compile *The Rust Book* and *mdbook* documentation without any errors or warnings (e.g. missing Unicode characters). See [Status of Rust Bookshelf](#status-of-rust-bookshelf) for up to date progress.
- [ ] Put "tectonic" dependency in "pdf" feature configuration.
- [ ] Add "table of contents" mdbook toml option.
- [ ] Add "markdown" mdbook toml option.
- [ ] Add "number of words" mdbook toml option.
- [ ] Add "examples" directory.
- [ ] Create documentation and move relevent docs to md2tex.
- [ ] Add option for custom LaTeX headers.
- [ ] Add option for alternative markdown-to-latex converter plugin.
- [ ] Add test suites.
- [ ] Cross compile binaries ([trust](https://github.com/japaric/trust))
- [ ] Add option to generate PDF with [mdproof](https://img.shields.io/badge/crates.io-v0.1.2-orange.svg?longCache=true) to skip LaTeX dependencies.

## See Also

The following projects served as guidance for `mdbook-latex` (or are simply cool enough that they deserve to be shared!):

- [mdbook-epub](https://github.com/Michael-F-Bryan/mdbook-epub): A backend for mdbook that creates EPUB files.
- [mdbook-linkcheck](https://github.com/Michael-F-Bryan/mdbook-linkcheck): A backend for `mdbook` that will verify URL links.
- [LaTeX-rs](https://github.com/Michael-F-Bryan/latex-rs): A cool library for programmatic LaTeX generation that I hope to eventually incorporate.
- [crowbook](https://github.com/lise-henry/crowbook/): A rich program that can generate HTML, PDF, **and** EPUB files from markdown code. Has a neat [online demo page](http://vps.crowdagger.fr/crowbook/) to try it out interactively. Similar in some respects to `mdbook`, but with an added focus on "novels and fiction". Though general enough to handle a lot of different projects.
- [no starch press](https://nostarch.com/Rust2018): *The Rust Programming Language* made professionally by a proper publishing company. Guranteed to have fewer errors than `mdbook-latex`!
