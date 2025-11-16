Cell1: Community Detection and Visualization
This cell defines the SpectralCommunityDetector class and runs the full algorithm on the Karate Club graph. It prints the improving modularity score at each successful iteration and generates three plots to visualize the process:

Initial State: The graph as one single community.

Intermediate State: The graph after several splits.

Final State: The final community structure with the highest modularity.

Cell 2: Node Centrality Analysis
This cell analyzes how the "importance" of each node changes as the communities are split. It generates 34 separate plots (one for each node) that track four different centrality metrics over the course of the algorithm:

Degree Centrality

Betweenness Centrality

Closeness Centrality

Clustering Coefficient

Analysis of Findings
This analysis reveals how a node's role changes based on its community.

Stable Nodes: Nodes 0 and 33 (the administrator and instructor) remain the most central figures in their respective groups throughout the entire process.

Betweenness Centrality: This metric sees the most change. Nodes that act as "bridges" between groups start with high betweenness, but this score plummets as soon as the algorithm "cuts" the connection and separates their groups.

Closeness Centrality: This often increases for nodes. As they end up in smaller, more tightly-knit communities, their average distance to other nodes within that community decreases.

Degree Centrality: This is the most stable metric, as it only depends on a node's immediate neighbors, which don't change.
