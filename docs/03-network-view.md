# Network View

## Objective

The Network View provides an interactive graph-based representation of a design document. It enables users to examine the entities contained in a design and the relationships between them at different levels of abstraction.

In this section, the same SBOL design will be examined using three different representations:

- **Top-Level View**
- **Hierarchical View**
- **Raw Graph View**

Comparing these representations demonstrates how SynBioKit can provide both simplified design-oriented views and detailed representations of the underlying SBOL structure.

---

## Example Design

This section uses the following SBOL document:

**`BBa_F2620_PoPSReceiver.ttl`**

[Open the example file](../examples/BBa_F2620_PoPSReceiver.ttl)

The document represents an SBOL design that will be used throughout this section to demonstrate the different Network View representations.

---

## Loading the Design

1. Open SynBioKit in a web browser.
2. Open `BBa_F2620_PoPSReceiver.ttl` from the tutorial repository.
3. Copy the complete contents of the file.
4. Paste the content into the input panel on the left-hand side of SynBioKit.

After the design is processed, SynBioKit automatically displays the document in the **Network View**.

The Network View represents SBOL entities as nodes and the relationships between them as edges.

---

# Top-Level View

## Overview

The Top-Level View provides a simplified representation of the SBOL document by displaying its principal design entities while hiding lower-level structural details.

This representation is useful for obtaining an initial overview of a design without exposing every entity and relationship contained in the underlying SBOL document.

## Procedure

1. Ensure that `BBa_F2620_PoPSReceiver.ttl` is loaded in SynBioKit.
2. Select **Top-Level View** from the available Network View options.
3. Examine the entities displayed in the graph.
4. Select individual nodes to inspect the corresponding SBOL entities.

## Expected Outcome

The graph should provide a concise representation of the Top Level entities contained in the design.


> **Observation**
>
> Identify the principal entities visible in the graph. Consider which information from the original SBOL document is not represented in this view.

[Top-Level View](assets/images/toplevel.png)

---

# Hierarchical View

## Overview

The Hierarchical View represents the design according to its structural hierarchy.

Rather than displaying every SBOL object independently, this view emphasises the relationships between biological design entities and their contained or associated elements.

It provides a top-down representation of the design and is particularly useful for understanding how complex designs are organised.

## Procedure

1. Change the Network View representation to **Hierarchical View**.
2. Examine how the structure differs from the Top-Level View.
3. Identify parent and child relationships within the design.
4. Select different entities to examine their position within the hierarchy.

## Expected Outcome

The design should now be represented as a hierarchical structure.

The relationships between higher-level design entities and their associated elements should be more explicit than in the Top-Level View.

> **Observation**
>
> Compare the hierarchical representation with the Top-Level View. Identify which structural relationships become visible when the hierarchy of the design is considered.

<!-- Add screenshot here -->
<!-- ![Hierarchical View](assets/images/network-hierarchical.png) -->

---

# Raw Graph View

## Overview

The Raw Graph View provides the most detailed graph representation available in the Network View.

It exposes the SBOL entities and relationships derived directly from the document structure, with substantially less abstraction than the Top-Level or Hierarchical representations.

This view is useful when detailed inspection of an SBOL document is required.

## Procedure

1. Change the representation to **Raw Graph View**.
2. Examine the number and types of nodes displayed.
3. Inspect the relationships connecting the entities.
4. Select several nodes and compare them with the corresponding information in the original SBOL document.

## Expected Outcome

The graph should contain considerably more detail than the previous two representations.

Entities and relationships that were hidden or abstracted in the Top-Level and Hierarchical views should now be visible.

> **Observation**
>
> Compare the Raw Graph View with the previous representations. Consider the trade-off between structural detail and readability.

<!-- Add screenshot here -->
<!-- ![Raw Graph View](assets/images/network-raw-graph.png) -->

---

# Comparison of Network Representations

The three Network View representations provide different levels of abstraction over the same SBOL document.

| View | Primary Purpose | Level of Detail |
| --- | --- | --- |
| **Top-Level View** | Provides an overview of the principal design entities | Low |
| **Hierarchical View** | Emphasises the organisation and hierarchy of the design | Medium |
| **Raw Graph View** | Exposes detailed SBOL entities and relationships | High |

The appropriate representation therefore depends on the type of analysis being performed.

The **Top-Level View** is suitable for rapidly identifying the main elements of a design, whereas the **Hierarchical View** provides additional information about design organisation. The **Raw Graph View** is intended for detailed inspection of the SBOL document and its underlying relationships.

---

## Section Summary

In this section, a single SBOL document was examined using three different Network View representations.

The exercise demonstrated how SynBioKit provides multiple levels of abstraction for analysing the same biological design:

**Top-Level View → Hierarchical View → Raw Graph View**

These representations allow users to move from a simplified overview of a design to a detailed examination of its underlying SBOL structure.

[Next: Validation →](04-validation.md)