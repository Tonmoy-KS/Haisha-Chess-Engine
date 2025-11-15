<div align="center">

  <!-- logo -->
  <img src="https://stockfishchess.org/images/logo/icon_128x128.png" alt="Haisha Logo">

  <h3>Haisha (敗者)</h3>

  A free and strong UCI chess engine... for finding the worst possible move.
  <br>
  <strong>[Explore Haisha's descent into madness »][wiki-link]</strong>
  <br>
  <br>
  [Report a good move][issue-link]
  ·
  [Open a discussion][discussions-link]
  ·
  [Discord][discord-link]
  ·
  [Blog][website-blog-link]

</div>

## Overview

**Haisha** (敗者, Japanese for "Loser") is a **free and strong UCI chess engine** derived from
Stockfish. It analyzes chess positions to compute the most mathematically disastrous move.

Haisha is an exploration into the concept that being perfectly bad requires a near-perfect
understanding of chess. To find the worst move, the engine must evaluate all possibilities,
calculate long-term consequences, and understand complex concepts... just to violate them optimally.

Haisha **does not include a graphical user interface** (GUI). To use it, you will need
a UCI-compatible GUI.

## Files

This distribution of Haisha consists of the following files:

  * [README.md][readme-link], the file you are currently reading.

  * [Copying.txt][license-link], a text file containing the GNU General Public License version 3.

  * [AUTHORS][authors-link], a text file with the list of authors for the project.

  * [src][src-link], a subdirectory containing the full source code.

  * a file with the .nnue extension, storing the neural network used for evaluation.

the main and almost only changes made to stockfish for Haisha is in the `search.cpp` search algorithm file.
## Contributing

__See the [Contributing Guide](CONTRIBUTING.md).__

### Improving the code

Haisha is a fork of Stockfish. To understand the original architecture, the
[chessprogramming wiki][programming-link] is an invaluable resource.

## Compiling Haisha

Haisha has the same compilation requirements as Stockfish. On Unix-like systems,
it should be easy to compile directly from the source code. An example:

```
cd src
make -j profile-build
```

Detailed compilation instructions can be found in the original
[Stockfish documentation][wiki-compile-link].

## Terms of use

Haisha is free and distributed under the
[**GNU General Public License version 3**][license-link] (GPL v3). It is a
derivative work of Stockfish. This means you are free to do almost exactly what you
want with the program, including distributing it or using it as a starting point for
a project of your own.

The only real limitation is that whenever you distribute Haisha, you MUST
always include the license and the full source code (or a pointer to it). If you
make any changes to the source code, these changes must also be made available
under GPL v3.

## Acknowledgements

The original Stockfish engine uses neural networks trained on [data provided by the
Leela Chess Zero project][lc0-data-link]. Haisha benefits from this same data to
inform its (inverted) evaluation.