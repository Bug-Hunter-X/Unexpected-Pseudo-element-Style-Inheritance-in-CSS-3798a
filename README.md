# Unexpected Pseudo-element Style Inheritance in CSS

This repository demonstrates a subtle bug in CSS where a pseudo-element's styling unexpectedly overrides a more specific selector.  This is an uncommon issue that can be difficult to debug, particularly in larger stylesheets.

## The Problem

The `bug.css` file showcases the issue. A `span` element within a container unexpectedly inherits a style from the container's `::before` pseudo-element, even though the `span` has a more specific selector. This behavior violates the expected CSS specificity rules.

## The Solution

The `bugSolution.css` file provides a fix. This demonstrates how to isolate the pseudo-element's styling from affecting the element's child elements.  The solution might involve more granular styling or alternative techniques to manage the pseudo-element's style impact.