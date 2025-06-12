# HiRa-GO: Hierarchical Rainbow Community Detection in Gene Ontology Networks

This repository contains the official implementation of the HiRa-GO algorithm proposed in the paper:

**HiRa-GO: A Hierarchical Rainbow Community Detection Algorithm for Gene Ontology Networks**  
[Author(s)], [Affiliation], 2025

## Description

HiRa-GO is a DFS-based algorithm designed to detect hierarchical communities in directed ontology networks. It assigns colors to nodes by traversing the graph in post-order and propagating color labels based on leaf and internal node structure.

The method is especially suitable for biological networks such as the Gene Ontology and achieves better interpretability and lower structural entropy than modularity-based algorithms like Louvain.
## How to Run

1. Install required packages:

```
pip install -r requirements.txt
```

2. Run the algorithm:

```
python HiRaGO.py
```

3. Or use the Jupyter Notebook:

```
jupyter notebook notebooks/demo.ipynb
```

## Evaluation

HiRa-GO was evaluated on the Gene Ontology dataset and compared with the Louvain algorithm. The proposed method showed significant improvements in structural entropy:

| Method   | Structural Entropy |
|----------|--------------------|
| Louvain  | 6.71               |
| HiRa-GO  | 3.23               |

## Dataset

The Gene Ontology dataset used in this study is in `go-basic.json` format and is available from the official GO website.

## Citation

If you use this repository in your research, please cite:

```
@article{yourname2025hirago,
  title={HiRa-GO: A Hierarchical Rainbow Community Detection Algorithm for Gene Ontology Networks},
  author={Your Name and Coauthors},
  journal={Journal Name},
  year={2025}
}
```

## License

This project is licensed under the MIT License.
