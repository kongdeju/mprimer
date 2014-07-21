---
title: "mprimer: a reliable, flexible and high-throughput multiplex PCR primer design software"
layout: page
---

Multiplex polymerase chain reaction (Multiplex PCR), defined as the simultaneous amplification of multiple regions of a DNA template or multiple DNA templates using more than one primer set (comprising a forward primer and a reverse primer) in one tube, has been widely used in several fields, including: pathogen identification, high throughput SNP genotyping, mutation analysis, gene deletion analysis, template quantitation, linkage analysis, RNA detection, forensic studies etc. The primer design for multiplex PCR is the key step and still remains a major challenge.

#### <i class="fa fa-star"></i> Hairpins

Primer hairpins structure.

#### <i class="fa fa-star"></i> Dimers

Primer-primer dimers, and genome-mediated dimers.

#### <i class="fa fa-star"></i> Specificity

Amplicon-amplicon interaction, background DNAs (e.g. human genome).


0. Simulation primer-target binding activity by thermodynamics
  
    Thermodynamics has been proved to be a reliable method to predict the oligo hybridization properties.

0. Primer misprimer, self dimers and cross dimers all of them were measured by thermodynamics in MPRIMER

0. Genome-wide checking the primer specificity and dimers

  A k-mer index algorithm was developed to speed up the binding sites search against the large genome database.

0. Genome-mediated dimers finding algorithm

  Thermodynamics was used to measure the stability of the misprimer and dimers

0. Has a virtual electrophoresis function to predict the mobility of amplicon

  Virtual agarose gel electrophoresis analysis of each amplicon to prevent the overlap bands

0. Designs a flexible plugin mechanism for easily extending the applications of MPRIMER

  With powerful parameters of Primer3, MPRIMER implements a flexible plugin mechanism, which can easily extend the applications of MPRIMER

  For example, with a simple script, users can extend the MPRIMER to design primers for SNP genotyping

0. Auto-groups templates into different tubes when they are incompatible

  In the case of incompatible templates (e.g. due to high sequence similarity), MPRIMER can separate them automatically

0. High-throughput primer design

  The MPRIMER pipeline enables design hundreds of primers automatically without any human interference.