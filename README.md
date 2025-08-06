# 📌 Locality Sensitive Hashing (LSH) for Approximate Nearest Neighbor Search

This project explores and benchmarks different methods for Approximate Nearest Neighbor (ANN) search, focusing on:

- **Spherical Locality Sensitive Hashing (LSH)**
- **Naive brute-force search**
- **FAISS IndexFlatL2 (Facebook AI Similarity Search)**

We evaluate and compare these methods in terms of **search accuracy**, **query runtime**, and **memory usage** on synthetic high-dimensional data using **Euclidean distance**.

## 📂 Project Structure

```
.
├── LSH.ipynb
├── acd.tsv #the course descriptions with course numbers
├── course_descroptions.csv #the processed course descriptions wiht course numbers
├── README.md
└── requirements.txt
```

## ⚙️ Installation

```bash
git clone https://github.com/yuuuuuu0276/Locality-Sensitive-Hashing.git
pip install -r requirements.txt
```


## 📊 Evaluation Metrics

- **Query Runtime**: Time to find neighbors per query  
- **Recall@K**: Fraction of true nearest neighbors found  
- **Memory Usage**: Memory footprint of indexing structure

## 📈 Sample Results

| Method           | Recall@10 | Avg Runtime (ms) | Memory (MB) |
|------------------|-----------|------------------|-------------|
| Naive Search     | 1.00      | 150              | 2           |
| Spherical LSH    | 0.82      | 7                | 10          |
| FAISS IndexFlatL2| 0.99      | 2                | 5           |

> Note: These numbers are illustrative only. Your results may vary depending on dataset size and parameters.

## 📚 References

- [Indyk & Motwani (1998)](https://dl.acm.org/doi/10.1145/276698.276876) – Approximate Nearest Neighbors via LSH  
- [FAISS Library](https://github.com/facebookresearch/faiss)  
- [LSH Tutorial by Mining of Massive Datasets (MMDS)](http://www.mmds.org/)

## 🧠 Author

**Yu Da**  
Cornell University, B.A./M.Eng in Computer Science  
Feel free to connect or reach out if you have questions!

## 📝 License

MIT License
