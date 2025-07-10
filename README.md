# Gene Expression Heatmap and Boxplot Analysis

This project was completed as part of the *R for Data Science* course during the MSc Bioinformatics programme at the University of Edinburgh (2024).

## Description

The analysis explores gene expression patterns across treatment groups using:

- Heatmaps (genes clustered, samples clustered)
- Boxplots (expression grouped by treatment)
- Expression data and annotations

## Inputs

Place all required files inside the `/data` directory:

| File name             | Description                              |
|-----------------------|------------------------------------------|
| `data_all.csv`        | Gene expression matrix                   |
| `gene_annotation.csv` | Metadata for genes (names, types)        |
| `sample_annotation.csv` | Sample-level metadata (treatment groups) |
| `genelist.txt`        | List of gene IDs to include in analysis  |

## Output

Knit the RMarkdown file to generate the report:
- `analysis.pdf` (or HTML/Word, based on output format)

## How to Run

1. Open the `.Rmd` file in RStudio  
2. Ensure all `/data` files are present  
3. Change knit output to the ouput version you prefer.
4. Click **Knit** or use:

```r
rmarkdown::render("analysis.Rmd", output_format = "pdf_document")
```

## 📌 Notes 
Data is log₂ transformed to stabilize variance

Annotations link expression to gene types (XA/XB/XC) and treatments (1–4)

Boxplots reveal inter-group expression differences

## License 
This code is intended for educational use only.