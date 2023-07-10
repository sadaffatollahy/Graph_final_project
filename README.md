# Graph_final_project
Graph classification and Graph regrssion:

Abstract:

To accurately predict molecular properties, it is
important to learn expressive molecular representations. Graph
neural networks (GNNs) have made significant advances in this
area.Inthis project we focus on graph classification and graph regression.

introduction :

In the context of molecular graphs, a graph is typically represented as a set of atoms (nodes) and bonds (edges) between them, where the atoms represent the elements that make up the molecule (e.g., carbon, hydrogen, oxygen), and the bonds represent the covalent bonds between the atoms. Graph neural networks (GNNs) can be used to learn expressive molecular representations from these graph structures.

In this project we have 2 dataset ,one of them is for classification task and the other is for regression task.first we need to know what they are!

Graph Classification:

Graph classification is a type of machine learning task in which a model is trained to classify graphs based on their structural properties. Unlike traditional machine learning tasks that operate on fixed-dimensional data, such as images or text, graph classification involves working with data that is represented as a graph, which is a collection of nodes (vertices) and edges that connect the nodes.

In graph classification, each graph is typically represented as an adjacency matrix or an edge list, which captures the pairwise relationships between the nodes in the graph. The goal of the model is to learn a function that maps the graph representation to a categorical label, indicating the class to which the graph belongs.

Graph classification has a wide range of applications, including chemical compound classification, protein function prediction, social network analysis, and citation network analysis, among others. It is a challenging task due to the complexity of graph data and the difficulty in extracting meaningful features from the graph structure. However, recent advances in deep learning and graph neural networks have led to significant improvements in graph classification performance, making it an active area of research in machine learning and artificial intelligence.

Chemical compound classification:

Chemical compound classification is an important application of graph classification in which machine learning models are trained to predict the properties of chemical compounds based on their molecular structure. In this context, each chemical compound is represented as a graph, where the nodes represent atoms and the edges represent chemical bonds between the atoms.

The molecular structure of a chemical compound can have a significant impact on its physical and chemical properties, such as solubility, reactivity, and toxicity. By training a machine learning model to classify chemical compounds based on their molecular structure, it is possible to predict their properties and identify compounds with desirable characteristics for specific applications, such as drug discovery or materials science.

Graph neural networks (GNNs) have proven to be a powerful tool for chemical compound classification due to their ability to model the complex relationships between atoms in a molecule. GNNs can learn to extract relevant features from the graph structure, such as the presence of certain substructures or the length and type of chemical bonds, and use these features to predict the properties of the compound.


Dataset:

The dataset for this task is BBBP.
BBBP (Blood–brain barrier penetration) dataset  comes from a recent study on the modeling and prediction of
barrier permeability. This dataset records whether a compound is permeable to the blood-brain barrier.
This dataset contains 2000 graphs or molecules with 127 vertex features, 12 edge features, and 200 molecular features , each of which is explained below.

![4](https://github.com/sadaffatollahy/Graph_final_project/assets/123890119/7e54538c-f42e-4100-810f-301f74567e2a)

In this GNN we use of cross entropy as loss function and ROC-AUC as metric and node features and edge features . finally resaults are in below:

![8](https://github.com/sadaffatollahy/Graph_final_project/assets/123890119/4133d113-0ba0-4c93-b955-abc8aaf05447)

 As you can see my best result is Model 5.

Graph Regression:

Graph regression is a type of machine learning technique that involves predicting a continuous output variable from a graph-structured input. In graph regression, the input data is represented as a graph, where the nodes represent entities and the edges represent the relationships between those entities. The goal of graph regression is to learn a mapping between the input graph and a continuous output variable, such as a numeric value or a vector.

Graph regression can be used in a variety of applications, such as drug discovery, materials science, and protein structure prediction. In drug discovery, for example, graph regression can be used to predict the binding affinity of a candidate drug molecule to a target protein, given a graph representation of the molecule and the protein.

Graph regression models can be constructed using a variety of machine learning techniques, such as graph neural networks (GNNs), kernel methods, and decision trees. GNNs are a popular choice for graph regression because they are designed to operate on graph-structured data and can learn hierarchical representations of the input graph. GNNs can be trained using various loss functions, such as mean squared error (MSE) or mean absolute error (MAE), and can be optimized using standard backpropagation techniques.

Dataset:

The dataset for this task is ESOL.
 ESOL is a small dataset consisting of water solubility data for some compounds.
Like the previous dataset this dataset contains 2000 graphs or molecules with 127 vertex features, 12 edge features, and 200 molecular features.

In this GNN we use of MSE as loss function and RMSE as metric and node features and edge features . finally resaults are in below:

![9](https://github.com/sadaffatollahy/Graph_final_project/assets/123890119/0fc0d7ac-3078-4757-ba43-5d8d707f952e)

 As you can see my best result is Model 4.
