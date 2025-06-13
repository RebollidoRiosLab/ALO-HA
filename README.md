# Allergy Linking Oncology Human Analyses (ALO•HA)

**ALO•HA** is an interactive **Shiny** application developed by the [RebollidoRiosLab](https://rebollidorioslab.com/)  
for the AllergoOncology research community. It enables exploration of allergy-related omics data in a publication-aware and biologically contextualized way.

🔗 **Access the live app**: [https://rebollidorioslab.shinyapps.io/aloha/](https://rebollidorioslab.shinyapps.io/aloha/)

---

## 🔍 Features

1. **Browse & Filter Publications**  
   Instantly filter studies by year range, publication type, cell origin, disorder, sample source, study design, and molecule sets.  

2. **Visualize Associations**  
   Explore network graphs and Sankey diagrams showing relationships between molecules, disorders, and sample sources.  

3. **Reactome Pathway Enrichment**  
   Run pathway enrichment analysis for any selected subset of molecules.  

4. **Dynamic Plots & Tables**  
   Every plot, network, Sankey, and data table updates **in real time** whenever you change **any** filter or selection.

---

### ⚙️ Real-Time Recalculation & Busy Indicator

As soon as a user adjusts any filter (e.g., year range, disorder, molecule), ALO•HA automatically recalculates and refreshes:
- Annual trends barplots  
- Association networks  
- Sankey diagrams  
- Pathway enrichment heatmaps  
- Downloadable data tables  

During recalculation, a **fulfilling-square spinner** overlays the entire app interface and disappears once **all** outputs have updated.

---

## 📂 Downloadable Data

This repository provides two curated CSV files supporting transparency and reproducibility of the ALO•HA Shiny app:

### 1. [`data/aloha_molecule_data.csv`](data/aloha_molecule_data.csv)

A molecule-centric summary containing **451 molecules**, annotated with:
- The **studies** in which they were reported  
- Corresponding **sample sources**  
- Associated **diseases**

This file is also available directly within the ALO•HA web application (*Help* tab → *FAQs* section).

---

### 2. [`data/aloha_articles_metadata.csv`](data/aloha_articles_metadata.csv)

Metadata for the **138 curated articles** used as the primary annotation source for ALO•HA. This selection is the input for all downstream analysis and corresponds to **Table S1** in our paper.

**Included fields:**
- `pmid` – PubMed ID  
- `pubmed` – Full PubMed citation  
- `year` – Publication year  
- `doi` – Digital Object Identifier  
- `pubtype` – Publication type (e.g., original research, review)  
- `disorder` – Allergy subtype or disease  
- `MeSH_IDs` – Associated MeSH terms  
- `abbrev` – Custom short name for article  
- `db` – Database origin (if applicable)  
- `source` – Text-mining or manual curation  
- `molecules` – Molecules identified in the study  
- `sample` – Sample type (e.g., blood, nasal fluid)  
- `cell_origin` – Cell-type origin (if available)  
- `gene_number` – Number of genes/molecules reported  
- `study_type` – Experimental design (e.g., case-control, cohort)

---

## 👩‍🔬 Who Should Use ALO•HA?

- **Immunologists** and **allergologists** exploring molecular underpinnings of allergic disorders  
- **Bioinformaticians** analyzing gene-pathway associations in allergy-oncology interfaces  
- **Researchers** seeking an interactive, publication-linked tool for filtering, visualization, and analysis of allergy-relevant data

---

## 📚 Citation

If you use this dataset or the ALO•HA app in your research, please cite the associated publication once it becomes available.

---

## ✉️ Contact

For questions, feedback, or requests for additional data, feel free to reach out to:

- **Rocio Rebollido-Rios:** [rocio.rebollido-rios@uni-koeln.de](mailto:rocio.rebollido-rios@uni-koeln.de)  
- **Andrea Escolar-Peña:** [andrea.escolarpena@ceu.es](mailto:andrea.escolarpena@ceu.es)


© 2025 Rebollido-Rios Lab. Released for academic research purposes.


