[![made-with-latex](https://img.shields.io/badge/Made%20with-LaTeX-1f425f.svg)](https://www.latex-project.org/) [![Build the slides](https://github.com/EagleoutIce/se-projects-2023-flowr/actions/workflows/compile.yaml/badge.svg)](https://github.com/EagleoutIce/se-projects-2023-flowr/actions/workflows/compile.yaml)

*The project is planned for the Winter semester 2023/24 at ulm university (see [here](https://www.uni-ulm.de/in/fakultaet/studium/inf-mi/studienplanung-se/apse/)).*

- [Erklärung des Projekts (Deutsch)](#erklärung-des-projekts-deutsch)
  - [Interaktive Visualisierung von Datenflussgraphen](#interaktive-visualisierung-von-datenflussgraphen)
  - [Layout erhaltende Rekonstruktion des Slices](#layout-erhaltende-rekonstruktion-des-slices)
- [Project Details (English)](#project-details-english)
  - [Interactive Visualization of Dataflow-Graphs](#interactive-visualization-of-dataflow-graphs)
  - [Layout-Preserving Slice Reconstruction](#layout-preserving-slice-reconstruction)


The presentation can be found [here](https://media.githubusercontent.com/media/EagleoutIce/se-projects-2023-flowr/gh-pages/presentation.pdf):

[<img src="https://github.com/EagleoutIce/se-projects-2023-flowr/blob/gh-pages/preview-1.png?raw=true" width="650"/>](https://media.githubusercontent.com/media/EagleoutIce/se-projects-2023-flowr/gh-pages/presentation.pdf)


## Erklärung des Projekts (Deutsch)

Program Slicing ist eine wichtige Technik um Menschen beim Verständnis von Programmcode zu unterstützen.
Ein Program Slicer identifiziert für eine gegebene Variable die Teile des Programms, die einen Einfluss auf den Wert dieser Variable an der gegebenen Position haben können.
Das *flowR* Projekt konstruiert hierfür einen Datenflussgraphen, berechnet den Slice durch die Reduktion auf ein Erreichbarkeits-Problem und hat unter anderem das Ziel, ausführbaren Code zu erzeugen, der den Wert der gewählten Variable berechnet.
Um die Arbeit mit und die Ausgabe von *flowR* zu verbessern, gibt es zwei mögliche Projekte die hier angegangen werden können und die im Folgenden kurz beschrieben werden.

### Interaktive Visualisierung von Datenflussgraphen

![Studierende](https://badgen.net/static/Studierende/2%20-%204%20Studierende/blue?icon=codebeat&label=) ![Kontext](https://badgen.net/static/Kontext/Interaktive%20Visualisierung%20von%20Graphen/cyan?icon=bitcoin-lightning&label=) ![Ziel](https://badgen.net/static/Ziel/Webanwendung/grey?icon=rss&label=) ![AP SE](https://badgen.net/static/APSE/AP%20SE/green?label=) ![PSE1](https://badgen.net/static/PSE1/PSE1/green?label=) ![PSE2](https://badgen.net/static/PSE2/PSE2/green?label=)


[<img src="https://github.com/EagleoutIce/se-projects-2023-flowr/blob/gh-pages/preview-visualizer-1.png?raw=true" width="400"/>](https://media.githubusercontent.com/media/EagleoutIce/se-projects-2023-flowr/gh-pages/presentation.pdf)

Die von *flowR* generierten Datenflussgraphen erreichen schnell eine Größe, die mit statischen Visualisierungen wie zum Beispiel durch [Mermaid](https://mermaid.live) nicht mehr handhabbar ist.
Um die Arbeit mit diesen Graphen zu erleichtern sollen zwei bis vier Studierende eine interaktive web-basierte Visualisierung für *flowR* entwickeln, die die produzierten Datenflussgraphen darstellt und dem Nutzer diverse Operationen wie das Filtern und Ausblenden von Knoten und Teilgraphen erlaubt.

### Layout erhaltende Rekonstruktion des Slices

![Studierende](https://badgen.net/static/Studierende/1%20-%203%20Studierende/blue?icon=codebeat&label=) ![Kontext](https://badgen.net/static/Kontext/Generierung%20von%20ausführbarem%20Code/cyan?icon=bitcoin-lightning&label=) ![Ziel](https://badgen.net/static/Target/TypeScript%20Implementation/grey?icon=typescript&label=) ![AP SE](https://badgen.net/static/APSE/AP%20SE/green?label=) ![PSE1](https://badgen.net/static/PSE1/PSE1/green?label=) ![PSE2](https://badgen.net/static/PSE2/PSE2/green?label=)

[<img src="https://github.com/EagleoutIce/se-projects-2023-flowr/blob/gh-pages/preview-reconstruct-1.png?raw=true" width="400"/>](https://media.githubusercontent.com/media/EagleoutIce/se-projects-2023-flowr/gh-pages/presentation.pdf)

Das Slicing in *flowR* selektiert eine Menge an Knoten des [abstrakten Syntaxbaums](https://en.wikipedia.org/wiki/Abstract_syntax_tree), die für den Slice enthalten sein müssen. Eine bestehende Implementation in [TypeScript](https://www.typescriptlang.org/) versucht bereits auf Basis dieser Knoten, ausführbaren Code zu generieren, der den Wert der gewählten Variable berechnet und so nah wie möglich am ursprünglichen Layout des Programms ist. Die Ergebnisse sind dabei aber oft noch unzureichend, da beispielsweise eine Umformatierung des Codes stattfindet oder der Code nicht mehr ausgeführt werden kann.
Die Studierenden können im Rahmen des Projektes die bestehende Implementation erweitern oder eine neue Implementation entwerfen um die Qualität der generierten Ausgabe zu verbessern.

## Project Details (English)

Program slicing is an important technique to assist program comprehension.
A program slicer identifies the parts of a program, that can have an affect on the value of a variable at a given position.
To generate the slice, the *flowR* project uses a dataflow graph, reducing the challenge to a reachability problem, to produce executable code that calculates the value of the selected variable.
To improve working with and the output of *flowR*, I propose two possible projects that are described briefly in the following.

### Interactive Visualization of Dataflow-Graphs

![students](https://badgen.net/static/students/2%20-%204%20students/blue?icon=codebeat&label=) ![context](https://badgen.net/static/Context/interactive%20graph%20visualization/cyan?icon=bitcoin-lightning&label=) ![Ziel](https://badgen.net/static/Ziel/web%20application/grey?icon=rss&label=) ![AP SE](https://badgen.net/static/APSE/AP%20SE/green?label=) ![PSE1](https://badgen.net/static/PSE1/PSE1/green?label=) ![PSE2](https://badgen.net/static/PSE2/PSE2/green?label=)

[<img src="https://github.com/EagleoutIce/se-projects-2023-flowr/blob/gh-pages/preview-visualizer-1.png?raw=true" width="400"/>](https://media.githubusercontent.com/media/EagleoutIce/se-projects-2023-flowr/gh-pages/presentation.pdf)

*flowR*'s dataflow graphs scale quickly in size, rendering static visualization with tools like [Mermaid](https://mermaid.live) infeasible.
Hence, two to four students should develop an interactive web-based visualization for *flowR* that displays the produced dataflow graphs, allowing the user to perform operations like filtering and hiding nodes and subgraphs.

### Layout-Preserving Slice Reconstruction

![students](https://badgen.net/static/students/1%20-%203%20students/blue?icon=codebeat&label=) ![context](https://badgen.net/static/Context/generate%20executable%20code/cyan?icon=bitcoin-lightning&label=) ![Ziel](https://badgen.net/static/Target/TypeScript%20implementation/grey?icon=typescript&label=) ![AP SE](https://badgen.net/static/APSE/AP%20SE/green?label=) ![PSE1](https://badgen.net/static/PSE1/PSE1/green?label=) ![PSE2](https://badgen.net/static/PSE2/PSE2/green?label=)

[<img src="https://github.com/EagleoutIce/se-projects-2023-flowr/blob/gh-pages/preview-reconstruct-1.png?raw=true" width="400"/>](https://media.githubusercontent.com/media/EagleoutIce/se-projects-2023-flowr/gh-pages/presentation.pdf)

*flowR* slices by selecting a subset of nodes of the [abstract syntax tree](https://en.wikipedia.org/wiki/Abstract_syntax_tree) of the program.
There is already an existing implementation in [TypeScript](https://www.typescriptlang.org/) that tries to generate executable code which calculates the value of the selected variable while preserving the original layout of the program.
However, the results are often unsatisfactory, for example, due to the generated code being often reformatted or no longer executable.
Within the project, the students can choose to reuse the existing implementation or to create a new one, to improve the quality of the generated output.
