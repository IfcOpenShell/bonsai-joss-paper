---
title: 'BlenderBIM Addon: A system for detailed and data-rich OpenBIM IFC models'
tags:
  - Construction
  - Industry Foundation Classes
authors:
  - name: Dion Moult
    corresponding: true
    equal-contrib: true
    affiliation: "1" # (Multiple affiliations must be quoted)
  - name: Thomas Krijnen
    affiliation: 2
  - name: More people
    affiliation: 3
affiliations:
 - name: Something
   index: 1
 - name: Else
   index: 2
 - name: Here
   index: 3
date: 2 June 2023
bibliography: paper.bib

---

# Summary

Building Information Modeling (BIM) is a fairly recent paradigm shift in the exchange of construction information where information about construction works is no longer represented as symbolic 2d drawings but instead as computer interpretable object models. The Industry Foundation Classes (IFC) are the predominant open standard for exchanging such models, consisting of a classification taxonomy for BIM objects, their representations, meta-data and relationships. As such, it is also suitable for use as a primary project database rather than as simply a transfer medium.

BlenderBIM is a Native IFC Editor and BIM authoring tool. Although legacy BIM software applications share many concepts, they have limited scope for interoperability due to the use of proprietary undocumented file formats. In contrast, BlenderBIM uses IFC natively as its data store, preventing a lossy import/export step.

# Statement of need

BlenderBIM demonstrates that Native IFC editing is a viable software pattern with a number of advantages over legacy approaches:

- A Native IFC tool doesn't need to understand or process all data, however it must preserve data it doesn't use. This principle of data integrity means that BlenderBIM is usable as a professional tool from day one. Contrary to traditional tools where the import process discards all information that cannot be mapped to the native internal model.

- Native IFC editing is fast as there is no import/export conversion process involved. Partial loading possible.

- IFC files edited in BlenderBIM are versionable (by means of constructs in the schema), it is easy to see exactly what has changed between any two versions of the same project. (TK: traditional tools have also demonstrated this ability)

- IFC step files are text files with each entity on a separate line. BlenderBIM makes local changes to these files, allowing efficient storage, retrieval and sharing using the Git revision control system. BlenderBIM provides a collaborative branch and merge workflow similar to modern software development practices.

- The full breadth of IFC schema at the disposal of users and developers. Making it suitable for classroom usage and rapid prototyping.

[v] NativeIFC, truthful representation of IFC instead of import/export

Drawing generation and other downstream outputs

Relevance to education

Relevance to academia

# Approach

C++ | Python | hl api | blenderbim

Interesting details

# Domains

## Costing

## Sequencing

## Structural

## Thermal analysis

# Storage

## ifc+git

## ifc+edgedb

# Acknowledgements

# References
