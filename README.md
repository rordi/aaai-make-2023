# AAAI-MAKE 2023

Paper and slides from the AAAI-MAKE 2023 contribution on applying machine learning and knowledge graphs
in the domain of the Reviewer Assignment Problem (RAP).

## Find Bias-Free Reviewers

The Reviewers App allows you to find potential, bias-free referees for your journal manuscripts using
semantic text similarity (STS) matching and automated conflicts-of-interest (CoI) resolution of potential
referees with the manuscript's authors.

This is a prototypical system for evaluation purposes which is part of a research project at the University
of Applied Sciences and Arts Northwestern Switzerland (FHNW). The prototype includes open publication data
from MDPI for 2020-2021 (ca. 370K journal articles).

Usage
you provide the manuscript data (title, abstract, authors)
the system will find semantically related papers from the literature
the system will consider authors of semantically related papers as potential reviewers
you define the papers / potential reviewers to keep in the pool
the system will resolve the potential conflicts-of-interest for each potential reviewer in the pool (co-authorship, 2nd-level co-authorship, and frequent institute-to-institute collaborations)
the system will recommend potential reviewers that have the least (or no) conflicts of interest
To find potential bias-free reviewers for a manuscript, you will need to provide the manuscript data to the system:

Title and/or abstract [required, will not be saved]
E-mail addresses of the manuscript co-authors [required, will not be saved]
