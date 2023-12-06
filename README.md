# A Hybrid Intelligent Approach Combining Machine Learning and a Knowledge Graph to Support Academic Journal Publishers Addressing the Reviewer Assignment Problem (RAP)

## AAAI-MAKE 2023

Paper and slides from the AAAI-MAKE 2023 contribution on applying machine learning and knowledge graphs
in the domain of the Reviewer Assignment Problem (RAP).

- Slides: https://github.com/rordi/aaai-make-2023/blob/main/slides.pdf
- Preprint: https://github.com/rordi/aaai-make-2023/blob/main/paper.pdf

## Find Bias-Free Reviewers

The Reviewers App allows you to find potential, bias-free referees for your journal manuscripts using
semantic text similarity (STS) matching and automated conflicts-of-interest (CoI) resolution of potential
referees with the manuscript's authors.

This is a prototypical system for evaluation purposes which is part of a research project at the University
of Applied Sciences and Arts Northwestern Switzerland (FHNW). The prototype includes open publication data
from MDPI for 2020-2021 (ca. 370K journal articles).

## Solution Documentation

The system is composed of several components:

- **Vector Search Engine:** is an index of document embeddings created with Allen AI SPECTER of past scholarly publications. The component supports approximate nearest neighbours (ANN) search through the implementation of the Hierarchical Navigable Small World (HNSW) algorithm.
- **Graph Database:** graph representation of past publications, including the co-authorship network and institutional affiliations. The component supports the resolution of conflicts-of-interest between potential reviewers and authors (direct co-authorship, second-level co-authorship, and institute-to-institute collaborations).
- **Backend Application:** backend application in Python offering API endpoints to access business logics, to compute document embeddings with SPECTER, and to access data from the other layers (graph database, vector search).
- **Frontend Application:** frontend with graphical user interface for journal editors to use.
