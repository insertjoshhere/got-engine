# got-engine
An advanced reasoning engine that transforms highly complex, non-linear text analysis tasks into a Directed Acyclic Graph (DAG) of logical steps, letting an LLM explore multiple reasoning pathways.

## Summary
got-engine is a search-driven reasoning framework that implements advanced test-time compute scaling for highly complex, non-linear text analysis tasks. By breaking down reasoning workflows into a Directed Acyclic Graph (DAG) of logical thoughts rather than a straight-line sequence, got-engine allows text APIs to generate alternative hypotheses, aggregate insights across distinct logical pathways, and programmatically backtrack when a deduction hits a dead end.

## Project Goals & Technical Scope
The goal of this project is to implement academic research paradigms directly into the corporate software layer, covering:

* Custom Graph-State Tracking: A pure Python DAG management layer designed to handle text nodes, state tracking, and edge transformation properties.

* Search-Space Heuristics (BFS/DFS): Algorithms that control the generation and branch-expansion velocity of LLM thought steps.

* Programmatic Critic & Evaluation Nodes: Fast, cost-efficient evaluation heuristics and verification prompts that score the logical validity of generated reasoning steps against baseline constraints.

* Automatic Backtracking Routines: Mechanisms that intercept low-confidence nodes, prune the entire sub-tree, roll back state to the parent node, and prompt the generator for alternative analytical directions.

## Business & Application Context
This engine targets mission-critical corporate decision-support rooms, complex supply chain logistics, and high-stakes auditing environments (such as contract compliance, insurance appeals processing, or network configuration analysis). In these fields, simple linear prompt engineering fails because business problems possess deep structural dependencies—a choice made in step two might violate a contractual clause analyzed in step ten. This framework is deployed to handle highly ambiguous, multi-factor problem spaces. It forces the language model to systematically draft multiple parallel analytical branches, score the logical and legal validity of each deduction against deterministic corporate parameters, prune non-viable options early, and backtrack to explore alternative logical solutions, ultimately delivering a legally defensible, zero-hallucination execution path.

## Architecture
https://drive.google.com/file/d/12HO5uFq0cD988pa0tZVA7Ri1smiqfKqu/view?usp=sharing
