# MathJax Option

A MathJax configuration file providing custom TeX macros inspired by the LaTeX `physics` package. This configuration extends MathJax with convenient shortcuts for commonly used mathematical notation in physics, engineering, and applied mathematics.

## Features

### Number Sets

Standard mathematical number set symbols:

| Macro | Output |
|-------|--------|
| `\N` | Natural numbers |
| `\Z` | Integers |
| `\Q` | Rational numbers |
| `\R` | Real numbers |
| `\C` | Complex numbers |

### Automatic Bracing

Macros for automatic delimiter sizing:

| Macro | Description |
|-------|-------------|
| `\qty{x}` | Parentheses |
| `\pqty{x}` | Parentheses |
| `\bqty{x}` | Square brackets |
| `\Bqty{x}` | Curly braces |
| `\vqty{x}` | Vertical bars |
| `\abs{x}` | Absolute value |
| `\norm{x}` | Norm |
| `\eval{x}` | Evaluated at |
| `\order{x}` | Big-O notation |
| `\comm{A}{B}` | Commutator |
| `\acomm{A}{B}` | Anticommutator |
| `\pb{A}{B}` | Poisson bracket |

### Vector Notation

| Macro | Description |
|-------|-------------|
| `\vb{v}` | Bold vector |
| `\va{v}` | Arrow vector |
| `\vu{v}` | Unit vector |
| `\vdot` | Dot product |
| `\cross` | Cross product |
| `\grad` | Gradient |
| `\div` | Divergence |
| `\curl` | Curl |
| `\laplacian` | Laplacian |

### Operators

Trigonometric, hyperbolic, and other operators with automatic parentheses:

- Trigonometric: `\sin`, `\cos`, `\tan`, `\csc`, `\sec`, `\cot`
- Inverse: `\arcsin`, `\arccos`, `\arctan`, `\asin`, `\acos`, `\atan`
- Hyperbolic: `\sinh`, `\cosh`, `\tanh`, `\csch`, `\sech`, `\coth`
- Other: `\exp`, `\log`, `\ln`, `\det`, `\Pr`, `\tr`, `\Tr`, `\rank`, `\erf`, `\Res`, `\Re`, `\Im`

### Derivatives

| Macro | Description |
|-------|-------------|
| `\dd{x}` | Differential |
| `\dv{f}{x}` | Derivative |
| `\pdv{f}{x}` | Partial derivative |
| `\fdv{f}{x}` | Functional derivative |
| `\var` | Variation |

### Dirac Bra-Ket Notation

| Macro | Description |
|-------|-------------|
| `\bra{\psi}` | Bra |
| `\ket{\psi}` | Ket |
| `\braket{\phi}{\psi}` | Inner product |
| `\ketbra{\psi}{\phi}` | Outer product |
| `\ev{A}` | Expectation value |
| `\mel{\phi}{A}{\psi}` | Matrix element |

### Quick Quad Text

Convenient spacing macros for conditions in equations:

`\qif`, `\qthen`, `\qelse`, `\qotherwise`, `\qand`, `\qor`, `\qfor`, `\qall`, `\qgiven`, `\qusing`, `\qsince`, `\qlet`

### Matrix Macros

| Macro | Description |
|-------|-------------|
| `\mqty{...}` | Parenthesized matrix |

## Usage

Include the configuration file in your HTML:

```html
<script type="text/x-mathjax-config" src="MathJaxOption.js"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.7/MathJax.js?config=TeX-AMS_HTML"></script>
```

Or inline the configuration before loading MathJax.

## Configuration Details

This configuration sets:

- HTML-CSS scale: 120%
- Inline math delimiters: `$latex...$`, `$LATEX...$`, `\(...\)`
- Display math delimiters: `$$...$$`, `\[...\]`
- TeX extensions: color, AMSmath, AMScd, enclose
- Automatic equation numbering (AMS style)

## License

See the repository for license information.
