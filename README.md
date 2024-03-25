# Statistical Inference for Spatial Regionalization (SISR) Project - DBMS CS236 - UCR

## Overview
This project is a reimplementation and extension of the methodologies introduced in the research paper "Statistical Inference for Spatial Regionalization" by Hussah Alrashid, Amr Magdy, and Sergio Rey. The foundational aim of this work is to tackle the challenge of spatial regionalization, which involves clustering spatial areas into contiguous regions under specific cardinality constraints. By employing the P-Regionalization through Recursive Partitioning (PRRP) technique, our project not only seeks to recreate the novel approach for generating statistically significant regionalization solutions as proposed in the original study but also aims to broaden its application scope. A significant extension of this project is the development of a new module designed specifically for implementing the PRRP algorithm within graph data structures. This enhancement aims to demonstrate the versatility of the PRRP algorithm, showcasing its efficacy not just in spatial data but also in graph-based representations, thereby opening new avenues for statistical inference in spatial regionalization problems.

## Motivation
Spatial regionalization plays a crucial role in various domains, including land-use allocation, healthcare resources distribution, and community detection. Given the NP-hard nature of regionalization problems, existing algorithms offer approximate solutions. This project aims to generate random sample solutions with predetermined region cardinalities to facilitate statistical inference on any given regionalization scheme, enhancing the quality assessment of these approximations.

## Methodology
The project employs a parallel technique named PRRP, which operates over three phases:
- **Region Growing Phase**: Constructs initial regions with predefined cardinality.
- **Region Merging Phase**: Ensures the spatial contiguity of unassigned areas, allowing for the subsequent growth of regions.
- **Region Splitting Phase**: Adjusts the sizes of the initial regions to meet the predefined cardinalities precisely.

This methodology ensures that unassigned areas remain spatially contiguous, significantly improving the probability of generating feasible and statistically significant sample solutions.

## Implementation Details
The project is divided into two main Jupyter Notebook files:
- `PRRP-implementation.ipynb`: Contains the implementation of the PRRP algorithm, including preprocessing steps, region growing, merging, and splitting phases. It utilizes libraries such as Pandas, Geopandas, NetworkX, Fiona, and Matplotlib for data manipulation and visualization.
- `graph-final.ipynb`: Demonstrates the application of the PRRP algorithm on graph data structures, highlighting its versatility and efficiency in partitioning graph-based spatial data.
