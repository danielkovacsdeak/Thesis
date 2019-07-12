# Thesis
### Virus epidemics modeling on Scale-free networks. Contains the graph builder, the spreading process simulator (SIS model), a graph visualisation tool and the thesis itself which is written in Hungarian ("Szakdolgozat.pdf").

The codes are in [Jupyter Notebooks](https://jupyter.org/), if github fails to display it you can use [nbviewer](https://nbviewer.jupyter.org/) instead. Copy the url from github and it will display the notebook.

The Network.ipynb generates a [Scale-free graph](https://en.wikipedia.org/wiki/Scale-free_network) using the [Barabasi-Albert-model](http://networksciencebook.com/). It builds a big graph to an initial graph you decide the number of new nodes in it. In every step the algorithm ads one node with a pre-set number of edges. In this notebook you can save the network to an adjacency list in txt format, the "Network visualisation.ipynb" uses this list to display the network.

The Epidemic.ipynb does the spreading process based on the [SIS-model](https://institutefordiseasemodeling.github.io/Documentation/general/model-si.html). You decide about the infection probability, the healing probability, the initial number of infected nodes and the length of the simulation. In every step it iterates over the nodes, if a node is infected then it draws on healing (with the pre-set healing probability), if it does not heal then it draws on infection for every single edge of the infeced node.

