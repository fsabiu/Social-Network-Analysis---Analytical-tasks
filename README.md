# Assignment 1: Network Analysis and Analytical Tasks

This assignment composes of 4 exercises.

- The data used as inputs must be stored (gzipped) in **data**;
- The code written to address each exercise must be stored into a dedicated folder (*exerciseN*, with N in [0, 3]).  
- The analytical results for each exercise must be stored (gizipped) in **results/exerciseN**;
- The plot produced must be stored in **plots**.

## Exercise 0: Network Analysis

The analysis can be performed either by using a visual tool (i.e., Cytoscape and Gephi) and/or the support of a programming language.
The use of python ([networkx](https://networkx.github.io/) or [igraph](https://igraph.org/python/)) is not mandatory, although, strongly suggested. 
 
Network analysis must include at least:
- Degree distribution analysis;
- Connected components analysis;
- Path analysis;
- Clustering Coefficient, Density analysis;
- Centrality analysis.

Moreover, the statistics computed on the crawled data must be compared with the ones of (i) random and (ii) preferential attachment graphs having the same
number of nodes and edges.

## Exercise 1-2: Analytical Tasks

Each group must address at least **two** among the following tasks:

1. **Community Discovery:**
Identify, evaluate and validate the modular structure of the crawled network sample. 
The results of *K-clique*, *Label Propagation*, *Louvain*, and *Demon/Angel* must be evaluated and compared.
If additional semantic information for the analysed graph are present use them to make sense of the identified partitions.
For CD algorithm implementations (as well as for their evaluation and comparison) refer to the [cdlib](https://github.com/GiulioRossetti/cdlib) library.
The analysis can be extended selecting approaches considered interesting among the one present in such library.

2. **Tie Strength:**
Define some strategies to compute tie strength and analyze the impact of strong/weak ties on the connectedness and resilience of the crawled
network.

3. **Spreading:**
Simulate, using the [ndlib](https://github.com/GiulioRossetti/ndlib) python library, the diffusion models discussed during the course (i.e., SI, SIS, SIR and Threshold model) both on the
crawled data and on synthetic graphs (i.e., ER and BA).
Analyse the simulation results varying both model parameters and initial conditions (i.e., the infection seeds);

4. **Spreading 2:** 
Leveraging the Custom Model facility offered by [ndlib](https://github.com/GiulioRossetti/ndlib) design an ad-hoc, novel, diffusion model for the crawled graph. The model can be designed
to take advantage of both network topological characteristics as well as external semantic information attached to nodes/edges (if present). 
Define your model so to solve a specific diffusion problem you consider interesting for your data. 
The model can be either coded in python or expressed using NDQL. 
Analyse the results varying both model parameters and initial conditions (i.e., the infection seeds);

5. **Link Prediction:**
Partition each network in a training (80% of the edges) and a test set (20% of the edges) and apply some of the classical unsupervised link prediction approaches introduced in "David Liben-Nowell, Jon M. Kleinberg: The link prediction problem for
social networks. CIKM 2003" (i.e. Common Neighbors, Adamic Adar, Jaccard, Preferential Attachment). 
Discuss the prediction accuracy as done in the referenced paper.

## Exercise 3: Open problem

Define a research question on your data and use SNA tools to address it!

This final task requires you to:
- reason on the crawled data, 
- identify a concrete question to address, and 
- try to tackle it combining the technique discussed in class/implementing your own ideas/solutions.

If necessarily you can make use of additional data w.r.t. the network structure.

Examples of questions are:
- (Linkedin) Can we relate work mobility with social structure?
- (Twitter) How can we measure “polarization” in political debate?
- (Reddit) Can we identify trolls from their social neighborhood and posting activity?
- ...

