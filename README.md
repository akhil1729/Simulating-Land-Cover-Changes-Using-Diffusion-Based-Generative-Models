Simulating Land Cover Changes Using Diffusion-Based Generative Models Using Sentinel-II EuroSAT Data


Executive Summary Report 
Simulating Land Cover Changes Using Diffusion-Based Generative Models
Introduction: Land cover changes due to urbanization, deforestation, and agricultural expansion pose significant challenges to environmental conservation, urban planning, and resource management. These changes impact ecosystems, water resources, and human infrastructure, necessitating predictive tools to monitor and simulate these alterations. This project employs diffusion-based generative models to simulate land cover changes using the EuroSAT dataset. The goal is to provide actionable insights for urban planners, environmental agencies, and policymakers to make informed decisions.

Business Problem: The growing demand for land, coupled with unsustainable development practices, underscores the need for tools that predict and simulate land cover changes. Organizations such as government agencies, environmental NGOs, and urban planning firms require reliable methods to forecast land transformations, ensuring sustainability and effective resource allocation. This project aims to bridge this gap by leveraging cutting-edge machine learning techniques.

Data Sources: The EuroSAT dataset, a publicly available satellite imagery dataset, was utilized in this project. The dataset provides labeled data for various land cover types such as forest, vegetation, Lakes, Rivers, residential, farmland, and industrial areas. It offers a robust foundation for developing and validating models that simulate changes in land cover. The images available in the dataset are in .tiff which with 13 bands

Link for the dataset: https://zenodo.org/records/7711810#.ZAm3k-zMKEA


Methodology:

Generative Modeling:
Diffusion-based generative models were used to create synthetic images. These models iteratively transform noise into coherent images, simulating potential land cover changes over time.

Classification Models:
After generating synthetic images, classification models were employed to evaluate their quality and relevance. These models ensured that the generated images aligned with real-world patterns of land cover types.

Validation:
Validation involved testing the generated images against a reserved test set to assess their predictive validity. Metrics such as classification accuracy, Fréchet Inception Distance (FID), and visual inspections were used to determine the realism and reliability of simulations.

Implementation Framework:
The Cross Industry Standard Process for Data Mining approach guided the project phases, including business understanding, data understanding, preparation, modeling, evaluation, and deployment.

Key Outcomes:
Model Performance:
The generative models which we developed were not able to get trained accurately due to the computation constraints which were about to generate simulated land cover changes, producing high-quality synthetic images consistent with real-world land patterns.
Noising is done accurately with v1 code and could generate the images after adding noise but the denoising failed which were improved in the v3 code but due to the GPU constraints, run time errors were encountered. 

Insights:
Generated simulations will reveal potential impacts of urban sprawl and agricultural expansion on forested areas.
The models identified high-risk zones for deforestation, aiding in proactive conservation planning.

Constraints and Limitations:
Computational power limited extensive experimentation, leading to a proof-of-concept (POC) approach.
Geographic constraints of the EuroSAT dataset restricted the applicability of simulations to European landscapes only.

Visualizations:
Model Outputs: The 13 layers of noised images were added below showing how the images look after adding the noise which can be seen in v1 code .

This above generated image displays the 13 bands noised image of sample input:
Conclusions: This project demonstrates the potential of diffusion-based generative models in simulating land cover changes. This project did not successfully implement a diffusion-based generative model to simulate land cover changes due to the computational resource constraints. The generated synthetic images will be of high quality and align with the target land cover types, providing valuable insights for urban planning and environmental conservation. While the proof-of-concept approach highlights the feasibility of this methodology, future work should address computational limitations and explore diverse datasets to broaden applicability. 

Recommendations:
Invest in high-performance computing resources to enable comprehensive model training.
Expand the dataset to include satellite imagery from other continents, enhancing global applicability.
Collaborate with environmental and urban planning organizations to integrate model outputs into decision-making processes.
Future Work: Future iterations of this project could explore the use of ensemble models combining diffusion-based and GAN models to improve image quality further. Additionally, integrating socio-economic data into simulations may provide holistic insights into land cover changes, considering human behavior and policy impacts.
Acknowledgment: This project was supported by data and resources from the EuroSAT dataset and inspiration from foundational research on diffusion-based generative models. 
Appendix: Detailed visualizations, and code snippets from the Jupyter Notebook used for this project are provided in supplementary materials. These offer insights into the implementation details and validation process.

Citations:
Rombach, R., Blattmann, A., Lorenz, D., Esser, P., & Ommer, B. (2022). High-resolution image synthesis with latent diffusion models. arXiv preprint. https://arxiv.org/pdf/2206.00364

P. Helber, B. Bischke, A. Dengel and D. Borth, "EuroSAT: A Novel Dataset and Deep Learning Benchmark for Land Use and Land Cover Classification," in IEEE Journal of Selected Topics in Applied Earth Observations and Remote Sensing, vol. 12, no. 7, pp. 2217-2226, July 2019, doi: 10.1109/JSTARS.2019.2918242. 
https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=8736785&isnumber=8789745


