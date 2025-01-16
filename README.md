         Description
--------------------------

This is a set of Python codes for implementing microbial network of producing certain compounds by utilizing C1/C2 carbon source as a substrate. 

1. The network so developed is a weighted signed directed network. Nodes in the network are taken as C1/C2 substrates, micro-organisms utilizing a single or multiple substrate and produce value added products. 

2. Some products at higher titre have toxicity to the micro-organisms which pertaining to the inhbitory interactions (red color; hammer shaped or no arrow). 

3. Weights are taken into account based on the amount of ATP produced (edge width) or consumed (blue color edges). These weights are taken from enumerating the reactions available in the literature and hence may not be correct. It requires lot more attention about the product formation through engineered way. 

4. Two network is generated. One for the visualization of weighted network and other for analyzing a particular node properties.

Input files

1. list_microbes_C1C2_uptake_products.csv - Information about micro-organisms utlizing substrates along with some references.

2. microbial_network.ipynb - This is the main file as interactive file for Jupyter Notebook where all the codes along with functions are written. The codes first import the information and implement based on that. No or minimal hard wiring is done for curating the network. 

3. Microbial_network.py - This is the main .py file which can be run from terminal as well as spyder or any other UI. It generates .html file using pyvis package. It requires installation of pyvis "pip install pyvis" and import libraries from pyvis "from pyvis.network import Network". 

3. Improvement is needed to update the nodes position of the network.

4. Analysis of finding the efficient paths in the network for predicting the suitable consortia has not been done yet.
