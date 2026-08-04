---
layout: page
title: Denovo PiggyBac transposon generation
description: Apply genomic language models (e.g., evo2) for denovo PiggyBac transposon generation.
img: assets/img/PB_evo2.png
importance: 2
category: Ongoing
---
## Overview

We are designing de novo PiggyBac (PB) transposons using generative sequence models, pursuing two complementary strategies. 

1. We focus on the transposase protein itself, fine-tuning protein language models (e.g., ProGen2, ProtGPT3) on a large in-house PiggyBac dataset via SFT, then using reinforcement learning to align generated sequences with experimentally measured high-activity variants. 

2. We design the entire PB element from scratch using genomic language models (e.g., Evo2), fine-tuned on in-house PB data to generate complete transposon sequences de novo. 

Designs from both approaches are currently being validated experimentally in the lab.

