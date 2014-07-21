---
title: "mprimer: a reliable, flexible and high-throughput multiplex PCR primer design software"
layout: page
---

mprimer is a flexible and automatic pipeline for designing singleplex, multiplex, especially high-throughput (100+) multiplex PCR primers. It supports applications like multiple gene amplication at the same time, targets enrighment for next-generation sequencing (NGS), etc.

The target of multiplex PCR primer design is finding several primer pairs which can work compatibly in a tube, without hairpins, dimers, nonspecific amplications. Therefore, mprimer uses the cutting-edge research results for primer quality control. Besides, it also implements a flexible and smart algorithm to design thousands of primers automatically. Important features of mprimer including:

#### <i class="fa fa-star"></i> Check hairpins

The hairpin structure of each primer was checked by thermodynamics. Thermodynamics has been proved to be a more reliable method than sequence alignment algorithm for predicting the oligo hybridization properties, including hairpins, dimers, etc.

#### <i class="fa fa-star"></i> Check dimers

For each two primers in a tube, dimers between them, and thirdparty DNA (other than these two primers) assisted dimers will be check by thermodynamics.

#### <i class="fa fa-star"></i> Check specificity

For each two primers in a tube, nonspecific amplication among amplicons or background DNAs (DNAs other than template sequences, e.g. human genome) will be checked by thermodynamics. [MFEprimer](http://biocompute.bmi.ac.cn/CZlab/MFEprimer-2.0/) is our core product and been widely used in the world.

#### <i class="fa fa-star"></i> Check SNPs

There are two ways for avoiding SNPs sit in the 3'end of primers (e.g. the last 5 base region of a primer): 1) mask the regions before we design primers; 2) Let MFEprimer (version 3.0, not released to public now) check SNPs against the dbSNP database. The first way is fast and the last is suitable for existing primers.

#### <i class="fa fa-star"></i> Virtual electrophoresis

For low-throughput (usually < 20) multiplex PCR primer design, if amplicon size is the key for identifying amplicon, mprimer can control the amplicon size to avoiding the overlap bands.

#### <i class="fa fa-star"></i> Auto-group template sequences into different tubes

In the case of incompatible templates (e.g. high sequence similarity), mprimer can design primers and put them into different tubes.

#### <i class="fa fa-star"></i> Parallel for High-throughput primer design

Genome specificity checking is time-comsuming. It's an impossible mission if we use only single CPU for a 100-plex primer design task. mprimer speeds up by utilizing multiple CPUs of current computers.


---

### How to use?

Academic users, please go to [mprimer site](http://biocompute.bmi.ac.cn/CZlab/mprimer/).

Commercial users, please contact [me](http://mprimer.net/contact.html) for further information.