Changelog
---
All notable changes to the project will be documented in this file.

### [Unreleased](https://github.com/yudai-nkt/language-tex/compare/v0.4.0...master)
Please see the link above though it is not well summarized.

### [v0.3.1](https://github.com/yudai-nkt/language-tex/compare/v0.3.1...v0.4.0)
#### Changed
- Enhance the flexibility of TeX magic comment

### [v0.3.1](https://github.com/yudai-nkt/language-tex/compare/v0.3.0...v0.3.1)
#### Fixed
- Improper parsing of nested curly braces ([#11](https://github.com/yudai-nkt/language-tex/issues/11))

### [v0.3.0](https://github.com/yudai-nkt/language-tex/compare/v0.2.1...v0.3.0)
#### Added
- Grammar for Beamer's `\usetheme` and its components
- Grammar for single quotation

#### Changed
- Separate star from leading sectioning commands
- Distinguish function and variable in `expl3` syntax
- Remove two `invalid.illegal.string.quoted`s, which just do not get ligatured by LaTeX's feature
- Remove `meta.group.braces.tex` attribute

#### Fixed
- Improper parsing of cross reference commands ending with `ref` or `Ref`
- Unrecognized grammar of embedded sources in `lstlisting` environment
- Unrecognized expl3 syntax inside brackets ([#9](https://github.com/yudai-nkt/language-tex/issues/9))

### [v0.2.1](https://github.com/yudai-nkt/language-tex/compare/v0.2.0...v0.2.1)
#### Added
- Grammar for deprecated `eqnarray` environment

#### Fixed
- Improper parsing of `aligned`, `gathered` and `alignat`'s (optional) argument
- Unrecognized `minted` environment with preceding spaces ([#8](https://github.com/yudai-nkt/language-tex/pull/8))

### [v0.2.0](https://github.com/yudai-nkt/language-tex/compare/v0.1.1...v0.2.0)
#### Added
- Support for major languages' grammar in `minted` environment ([#5](https://github.com/yudai-nkt/language-tex/pull/5))
- Snippets for `figure` and `table` environment ([#6](https://github.com/yudai-nkt/language-tex/pull/6))
- Grammar for `\bibitem`
- Grammar for `\kcatcode`
- Snippet for `tabular` environment
- Snippets for `matrix` environment and its variants including `mathtools` extension

#### Changed
- Disable indent after `\begin{document}`
- Replace spaces in grammar files' name with hyphens
- Add tab stop at the location of environment's argument

#### Fixed
- Remove opening paren from matching for path of files loaded by the main source
- Matching for `\cite`'s argument
- Disable expansion of math snippets outside math mode ([area/language-latex#67](https://github.com/area/language-latex/issues/67))

### [v0.1.1](https://github.com/yudai-nkt/language-tex/compare/v0.1.0...v0.1.1)
#### Added
- Grammar for `\def` and its variants
- Grammar for definition macros provided by `xparse` package
- Grammar for deprecated font commands

#### Changed
- Naming of control sequences which start with `\Declare`

#### Fixed
- Relative links to `_img/preview.png` and `LICENSE.md`

### [v0.1.0](https://github.com/yudai-nkt/language-tex/compare/v0.0.0...v0.1.0)
#### Added
- Grammar for e-TeX's extended if-primitives
- Apply LaTeX Log grammar to log files generated by other than `pdftex` or `pdflatex`
- Grammar for control sequences which start with `\Declare`
- Matching for some non-ASCII characters inside the argument of `\label`, `\ref` and its variants ([area/language-latex#68](https://github.com/area/language-latex/issues/68))
- Support for `expl3` grammar ([area/language-latex#48](https://github.com/area/language-latex/issues/48))

#### Changed
- Refactoring of snippets

#### Fixed
- Grammar for `\iftrue`
- Grammar for `\providecommand`
- Escaped dollar sign in `minted` environment ([area/language-latex#75](https://github.com/area/language-latex/issues/75))
- Incorrect naming of `\label`'s argument ([#1](https://github.com/yudai-nkt/language-tex/pull/1))

### [v0.0.0](https://github.com/yudai-nkt/language-tex/compare/38c445d9bfe5abaa1703d01f95a7090726e1339e...v0.0.0)
This version is identical with the area's `language-latex` package as of August 2015 except for the following change:

- Updated `package.json` as a new package

Please refer to the original [CHANGELOG.md](https://github.com/area/language-latex/blob/38c445d9bfe5abaa1703d01f95a7090726e1339e/CHANGELOG.md) to see further history.