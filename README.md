# Inferring Gene Regulatory Networks from Omics Data 

## Objective
Uncover the dynamics of the major gene regulatory networks (GRN) involved in aging from single-cell omics data by applying a dynamical systems theory (DST) approach. DST is hereby choosen a framework, because of its potential to uncover the governing equations sturring the behavior of the system. The hope is, that this will allow modelling more complex relationships, then what would be possible using purely stocchastic approaches, while at the same time allowing much higher interpretability than what would be possible using a purely machine-learning based approach [[1](https://www.nature.com/articles/s41540-025-00565-3)]. The fundamental algorithm will be bassed on the concept of **Sparse Identification of Nonlinear Dynamics (SINDy)**, introduced by Brunton et al. (2016) [[2](https://www.pnas.org/doi/10.1073/pnas.1517384113), [3](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=7809160)]. 

The model will be applied to different **bone marrow** datasets. At first the processing and architecture of **implicit SINDy** [[3](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=7809160)] will adapted to be able to work with omics data, and evaluated by using it to infer the GRN of bone marrow differentiation, which should be simpler then uncovering the complex and also much more stacchastics based dynamics underlying aging. Afterwords the model will be applied to infer the GRN changes in mouse and human bone marrow aging.


## Steps
1. Infer GRN of bone marrow differentiation (mouse)
2. Infer GRN changes during bone marrow aging (mouse)
3. Infer GRN of aging on human bone marrow dataset

## Data
### GSE132042
Mouse Datasets (Bone Marrow) (10x and Smart-seq2) \
Part of the Tabula Muris Senis (TMS) dataset by CZ Biohub, a single-cell transcriptomics atlas covering data from 23 tissues and organs over the entire mouse lifespan. \
[Download](https://cellxgene.cziscience.com/collections/0b9d8a04-bb9d-44da-aa27-705bb65b54eb)

### GSE120221
Human Dataset (Bone Marrow) (10x) \
Data from 20 healthy adult human donors across a broad age range. \
[Download](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE120221)

<!-- ### GSE243327
Human Hematopoietic stem/progenitor cell (HSPC) Dataset (bulk RNA-seq?!) (young vs old) \
[Download](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE243327) -->

<!-- ### GSE264569
[Download](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE264569) -->

## Results

## Random Stuff
Then try to applying DST it to aging
- GSE127465: 
    - Human & Mouse
    - Single cell transcriptomics of human and mouse lung cancers reveals conserved myeloid populations across individuals and species

Hallmarks of Aging

- [ ] choose dataset (time-resolved RNA-seq)
- [ ] take major pathways for each of the hallmarks
- [ ] dimesionality reduction for each hallmark (PCA?)
- [ ] apply SINDy

## References
1. Islam, S. (2025). Dynamical systems theory as an organizing principle for single-cell biology. *npj Systems Biology and Applications, 11*, Article 85.
2. Brunton, S. L., Proctor, J. L., & Kutz, J. N. (2016). Discovering governing equations from data by sparse identification of nonlinear dynamical systems. *Proceedings of the National Academy of Sciences, 113*(15), 3932–3937.
3. Mangan, N. M., Brunton, S. L., Proctor, J. L. & Kutz, J. N. (2016). Inferring biological networks by sparse identification of nonlinear dynamics. *IEEE Transactions on Molecular, Biological and Multi-Scale Communications*, 2(1), 52–63. 
4. Khodaee, F., et al. (2025). The dissipation theory of aging: a quantitative analysis using a cellular aging map. *npj Aging*, 11, Article 86. 
5. Freitas, J. A. N. L. F. et al. (2023). Dynamic modeling of the cellular senescence gene regulatory network. *Heliyon*, 9(3), e14007. 
6. López-Otín, C. et al. (2023). *Hallmarks of aging: An expanding universe*, 186(2), 243-278.
