## Citation Regressor
In this section we want to create a model that can estimate how many citations a given paper 
will have based on its abstract, title, year, and author-author network.

### Regressor
```markdown
Top Predicted Citations:
                                                  title  year  \
6131  DSI-Net: Deep Synergistic Interaction Network ...  2021   
1077  Uni-ControlNet: All-in-One Control to Text-to-...  2023   
246   Anchor Diffusion for Unsupervised Video Object...  2019   

                 topic  predicted_citations  
6131               LLM         1.189171e+13  
1077  Diffusion Models         8.380618e+12  
246   Diffusion Models         3.803213e+12
```
### Author-Author Network
The idea is that scholarly paper authors have relations with each other that may be a great
predictor of how many citations a given paper is going to have.
```markdown
Test Set Regression Metrics:
RMSE: 144.20
MAE: 60.33
R2 Score: -0.27

Top Predicted Citations:
                                                   title  year  \
4119   The Good, the Bad, and the Expert: How Consume...  2015   
4740   Chinese Term Recognition and Extraction Based ...  2008   
4045   High efficient hardware allocation framework o...  2015   
10845  Score-Based Generative Modeling through Stocha...  2020   

                   topic  predicted_citations  
4119                 NaN          2697.807129  
4740                 NaN          2314.161621  
4045                 NaN          1178.770020  
10845   Diffusion Models          1175.487061
```