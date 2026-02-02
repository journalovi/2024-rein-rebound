# Real time, cross platform visualizations with zero dependencies for the N-body package REBOUND

An interactive article in the [Journal of Visualization and Interaction (JoVI)](https://journalovi.org/).

## Abstract

### Background
Visualizations have become an indispensable part of the scientific process. A vibrant ecosystem of visualization tools exists, catering to a wide variety of different needs. Real-time visualizations of numerical simulations offer scientists immediate feedback about the status of their simulations and can also be valuable educational and public outreach tools.

### Current Challenges
Developing a visualization tool with support for different operating systems, CPU/GPU architectures, and programming languages can be a challenge. It is common to use one or more UI toolkits or libraries to act as abstraction layers and hide the underlying complexity. Whereas external libraries greatly simplify the initial programming effort, we argue that relying on them introduces new dependencies and problems, such as a higher barriers to entry for new developers and users, and uncertainty regarding long-term support.

### Proposed Solution
In this paper we present a new approach for real-time visualizations which we have implemented for the N-body package REBOUND (Rein and Liu 2012). We propose to use a web browser to handle GPU accelerated rendering. This enables us to offer 3D, interactive visualizations of simulations running natively on all major operating systems. What makes our new approach unique is that we achieve this without the need for any external libraries. We utilize WebAssembly and emscripten to reuse existing OpenGL visualization code. Using communication via HTTP and a custom built-in web server, we are able to provide both local and remote real-time visualizations. In addition to the browser based real-time visualization, our approach offers other additional operating modes, including simulations running entirely within the browser, visualizations within jupyter notebooks, and traditional standalone visualizations using OpenGL. We focus on the implementation in REBOUND but the concepts and ideas discussed can be applied to many other areas in need of scientific and non-scientific real-time visualizations.

## Notes

Papers for this track are written in [Quarto](https://quarto.org/) which is an open source publishing format that supports inline code, including languages like R, Python, Julia, and JavaScript (via Observable Notebook).

Only edit .qmd files! The other files are generated from this.

```diff
Authors: @hannorein
OC: @mjskay
AE: @floe
R1: @RaphaelWimmer
R2: @sharponlooker
R3: @rmelikyan
AY: @domoritz
```
