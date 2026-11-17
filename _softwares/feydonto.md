---
layout: software
title: "FEYDOnto: An Aesthetic Ontology Visualizer"
excerpt: "An ontology viewer for making figures you can put in papers and demos: choose exactly which classes, properties and individuals to draw, then export a clean SVG or PNG."
logo: /images/feydonto-logo.png
meta: "Web app · JavaScript · RDF/XML, OWL, Turtle, N-Triples"
github: https://github.com/B-Gendron/feydonto
order: 1
author_profile: false
collection: softwares
---

<style>
.fo-colors { display: inline-block; width: 0.8em; height: 0.8em; border-radius: 2px; vertical-align: -0.05em; margin-right: 0.3em; }
</style>

FEYDOnto is an ontology viewer built for **figures**. You open an ontology, tick exactly the classes, properties and individuals you want to show, adjust the layout and style, and export a clean SVG or PNG ready for a paper, a poster or a slide.

The name stands for **F**igures **E**xactly as **Y**ou **D**esign them, from **O**ntologies. It is also the name of a very good cat.

## What it is for

Ontology editors such as Protégé show the whole ontology at once, which is fine for editing but rarely gives a figure you would put in a paper. FEYDOnto takes the opposite approach: **nothing is drawn unless you ask for it**. This makes it easy to show, for example, one branch of the class hierarchy, the two object properties that connect it, and three individuals out of ten thousand.

The output follows UML conventions: hollow arrows for subclasses, datatype properties as rows inside class boxes, restrictions (`some`, `only`, `min`, `max`) as labelled edges. The colours follow Protégé:
<span class="fo-colors" style="background:#e8a33d"></span>classes,
<span class="fo-colors" style="background:#2f6fd6"></span>object properties,
<span class="fo-colors" style="background:#2e9e4f"></span>datatype properties,
<span class="fo-colors" style="background:#8e44ad"></span>individuals,
<span class="fo-colors" style="background:#64748b"></span>annotations.

## Getting started

FEYDOnto is a static web page: there is nothing to install or build. You need:

- a recent browser (Chrome, Edge, Firefox or Safari, 2022 or newer);
- an internet connection, because the drawing libraries are loaded online;
- a small local web server, because browsers refuse to run the page from a `file://` address. Python 3 is enough.

```sh
git clone https://github.com/B-Gendron/feydonto.git
cd feydonto
python3 -m http.server 8000
```

Then open <http://localhost:8000> in your browser. Opening `index.html` by double-clicking it will **not** work.

## Quick start

1. Click **Open ontology…** (or drop a file on the window). To try the tool first, pick **Examples… › Pets**.
2. In the left panel, tick the classes you want in the **Classes** tab, then the properties and individuals in the other two tabs.
3. Drag nodes to adjust their position. Use the **Display** tab on the right to change the layout direction or spacing.
4. Pick a theme and a font in the **Style** tab (for a paper: *Paper* theme and *Serif* font).
5. In the **Export** tab, click **Download SVG** or **Download PNG**.
6. Click **Save view** to keep a `.json` file of your figure so you can reopen and edit it later.

## The interface

| Area | What you do there |
|---|---|
| **Top bar** | Open a file, load an example or a URL, search for an entity, undo / redo, save and load a view. |
| **Left panel** | Choose what to draw: the **Classes**, **Properties** and **Individuals** tabs list everything in the ontology with a checkbox. |
| **Canvas** (centre) | The figure. Drag nodes, zoom, double-click and right-click nodes to explore. |
| **Right panel** | **Inspect** the selected node or edge, set **Display** options and layout, change the **Style**, and **Export**. |

## Choosing what to draw

**Classes.** Ticking a class also ticks all its subclasses; **Shift+click** ticks only that class. The option at the top of the tab swaps these two behaviours. To keep a class but hide everything below it, click the **⊟** button at the end of its row.

**Properties.** Unticking a property removes it everywhere: edges, rows inside boxes and annotations.

**Individuals.** Tick only the ones you need. Ticking an individual also shows its class (you can turn this off in *Display › Other*).

Each tab has a filter field and **All** / **None** buttons. To find something quickly in a large ontology, press **/** and type its name in the search bar: choosing a result adds it to the figure.

**From the canvas.** Double-click a node to reveal its neighbours. Right-click it for more: *show subclasses / superclasses / individuals / connected nodes*, *isolate*, *hide*, *hide its subclasses*. Select a node and press **Delete** to hide it.

## Display options and layout

The **Display** tab controls what the boxes and arrows contain:

- **Relations to draw**: subclass, object property, restriction, instance-of, property assertion, equivalent class, disjoint with.
- **Contents of boxes**: datatype properties as rows in class boxes, data values in individual boxes, and whether an individual's class is shown as a dotted edge, a `: Class` caption, or both.
- **Annotations** (`rdfs:comment`, `skos:definition`, `dcterms:*`, any `owl:AnnotationProperty`): hidden, as a marker you hover to read, as text inside the box, or as a UML note. You can pick the language and cut long texts.
- **Edge labels**: optional text on subclass and instance-of arrows, such as `subClassOf`, `is-a` or `rdf:type`.
- **Names shown as**: `rdfs:label`, local name, or prefixed name (`ex:Thing`).

**Layout.** The default *Hierarchical* layout puts each level of the class hierarchy on its own row. *Tree*, *Organic* and *Radial* layouts are also available, with four directions and adjustable spacing. If you move nodes by hand, turn off *Re-layout automatically* so they stay where you put them while you add or remove things.

## Style

The **Style** tab offers four themes: *Paper* (print-friendly), *Vivid* (slides and demos), *Black & white* and *Dark*. You can also change the font (sans-serif, serif, monospace), the font size, the line width, straight or curved edges, each colour individually, and show a legend.

## Export

The export contains exactly what is on the canvas: hidden elements stay hidden.

- **SVG** (recommended): vector file with real, editable text. It opens in Inkscape, Illustrator and PowerPoint. For LaTeX, convert it with `inkscape --export-type=pdf figure.svg`.
- **PNG** at 1× (screen), 2× (slides) or 4× (print, about 300 dpi), or copied directly to the clipboard.

You can set the padding, a transparent background and whether to include the legend.

## Saving and sharing a figure

**Save view** writes a `.json` file with your selection, layout, node positions and style. To reopen it, load the same ontology, then click **Load view**. This makes figures reproducible: if the ontology changes, reload it and the view, and export again.

You can also open an ontology directly from a link by adding `?url=` to the address, for example `http://localhost:8000/?url=https://example.org/onto.ttl`.

## Shortcuts

| Action | Shortcut |
|---|---|
| Undo / redo | Ctrl/⌘+Z, Ctrl/⌘+Shift+Z |
| Search an entity | / |
| Hide the selected node | Delete |
| Deselect, close a menu | Esc |
| Tick a class without its subclasses | Shift+click |
| Reveal a node's neighbours | Double-click |
| More actions on a node | Right-click |

## Supported formats and limitations

FEYDOnto reads **RDF/XML** (`.rdf`, `.owl`), **Turtle** (`.ttl`) and **N-Triples** (`.nt`). Protégé's OWL/XML and Functional syntax are not supported yet: in Protégé, use *File › Save as* and choose RDF/XML or Turtle.

Not supported yet:

- JSON-LD and OWL/XML input;
- complex class expressions (other than simple restrictions) are shown as text in the inspector, not drawn;
- property hierarchies (`subPropertyOf`) are listed in the inspector only.

Bugs and suggestions are welcome on [GitHub](https://github.com/B-Gendron/feydonto/issues).
