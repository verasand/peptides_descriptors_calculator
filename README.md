# 🧬 Peptide Physicochemical Descriptor Calculator

This notebook calculates physicochemical descriptors for peptides from a FASTA file.

---

## 🔍 Features

- Calculates various physicochemical descriptors such as hydrophobicity, charge, and molecular weight.
- Includes QSAR descriptors and amino acid frequencies.
- Supports additional descriptors using the Peptidy library.
- Outputs results in a CSV file for further analysis.

---

## 📁 Expected Input Format

The input should be a `.fasta` file containing peptide sequences. Each sequence should have a unique identifier.

Example:

```
>Homo_sapiens|Insulin_B_chain|INS_HUMAN|30aa
FVNQHLCGSHLVEALYLVCGERGFFYTPKT
>Homo_sapiens|Glucagon|GCG_HUMAN|29aa
HSQGTFTSDYSKYLDSRRAQDFVQWLMNT
```

---

## ⚙️ How to Use

1. Install required packages: `peptides`, `peptidy`, `biopython`, `pandas`.
2. Upload a `.fasta` file containing peptide sequences.
3. Run the notebook cells to calculate descriptors and save the results.

---

## 📊 Example Output

The output is a `.csv` file containing the calculated descriptors for each peptide.

Example:

| ID                                   | Sequence                              | length_peptide | boman_index_peptides | hydrophobic_moment_peptides | hydrophobicity_index_peptides | charge_peptides | molecular_weight_peptides |
|-------------------------------------|--------------------------------------|----------------|-----------------------|-----------------------------|-------------------------------|-----------------|---------------------------|
| Homo_sapiens|Insulin_B_chain|INS_HUMAN|30aa | FVNQHLCGSHLVEALYLVCGERGFFYTPKT       | 30             | 0.549                | 0.491                       | 0.22                          | 0.057           | 3429.96                   |
| Homo_sapiens|Glucagon|GCG_HUMAN|29aa         | HSQGTFTSDYSKYLDSRRAQDFVQWLMNT        | 29             | 2.889                | 0.843                       | -0.99                         | 0.088           | 3482.79                   |

---

## ▶️ Launch in Google Colab

[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/verasand/peptides_descriptors_calculator/blob/main/descriptors_calculator.ipynb)

---

## 📄 License

MIT License  
© 2025 Sebastián Vera