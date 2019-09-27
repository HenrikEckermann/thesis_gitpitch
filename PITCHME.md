






@snap[mid]
#### Can fecal microbiota composition predict executive functioning in children?
@snapend

@snap[mid dtext text-07]
Henrik Eckermann
@snapend

@snap[south second-logo-sized]

@snapend

@snap[south-east second-logo-sized]
![](assets/img/dlogo.png) 
@snapend

@snap[south-west second-logo-sized]
![](assets/img/ruumc.png)
@snapend



---

## Introduction




Note:
1. What is the EF?
2. How could bacteria in the gut influence EF?
3. Previous research in that area
4. Societal and scientific relevance
5. Hypotheses

+++


## Executive functioning 






- initiation of goal-directed behavior  
- planning and organization  
- inhibition  
- flexible shifting  
- monitoring  
- working memory  
  

Note:
- Cognitive processes required for control of behavior most models include
- not exclusive to cognition


+++

@snap[north span-100]

## Gut Brain Axis  

@snapend

@snap[south span-50]
@img[span-80](assets/img/gutbrainaxis.png) 
@snapend

Note:  
- endocrine-, 
- neurocrine- and 
- immune-related signals that can influence the development and functioning of the brain


+++

## Previous research


- Animal studies ([Sarkar et al, 2018](https://www.ncbi.nlm.nih.gov/pubmed/29907531))
- Human study ([Carlson et al, 2018](https://www.ncbi.nlm.nih.gov/pubmed/28793975))



Note:  



Carlson:
- n = 89 infants, 86 for Mullen 1 year and 69 Mullen two year
- Mullen: 5 scales: gross motor, fine motor, visual reception, expressive language, receptive language. except the gross motor skill combined to Early learning composite score
- MB at 1 year age
- Mullen Scales of Early Learning + global and regional brain volumes using structural MRI at 1 + 2 years of age
- cluster analysis identiefied 3 groups
- Mullen scores at 2 years differed between clusters: C2 (high in Bacteroides) highest performance in 90th percentile, C1 (high levels of Faecalibacterium) lowest (72th percentile)
- higher alhpa diversity ;rarr& lower overall composite score at age 2
- minimal association between the gut microbiota and brain volume
- negative association between AD and ELC (5-23% variance explained) depending on index

Note on Mullen:
The Mullen has good standardization and reliability data, with median internal consistency scores ranging between 0.75 and 0.91, and test-retest correlations over 0.82 for 1-25 months


+++ 

## Animal studies

1. Stress and emotion 
2. Learning and memory
3. Social behavior
4. Autism 

@snap[south-east snap-pad-bottom-right span-20]
@img[border-img](assets/img/germ_free.png)
@snapend

Note:
To that extent, we describe microbial contributions to four phenomena of interest to cognitive scientists and psychologists, including (i) stress and emotion, (ii) learning and memory, (iii) social behavior, and (iv) autism.


Animal example:
- manipulation: probiotic/prebiotic/antibiotic + testing such as maze (e.g. Morris water maze) and/or inspection of brain tissue
- impairments in tests of memory and reductions in hippocampal BDNF in germ-free mice compared to normally colonized mice [74].
- rats administered ampicillin showed decreased spatial learning performance (and heightened anxiety) [75].
- compared to vehicle-treated rodents, mice and rats exposed to human milk oligosaccharides showed enhanced performance on a range of learning and memory tests, including working memory, spatial learning and memory, and learning via reinforcement [76].
- Investigations on infant rats showed similar effects of human milk oligosaccharides on novel object recognition, place and spatial memory, and long-term potentiation, benefits that were visible even 1 year after initial exposure to the prebiotic [77].



The hippocampus plays a crucial role in learning and memory, and its function in the generation and maintenance of spatial maps is especially well described in rodents [82].




+++



@snap[midpoint span-75]
## Human Study
@img[](assets/img/bio_psy.png)
@snapend

+++

@img[span-80](assets/img/carlson_cluster.png)


+++

@img[add-border-img span-60](assets/img/mullen_cluster.png)

+++

@img[add-border-img span-90](assets/img/mullensub_cluster.png)





+++

 

 


## Hypotheses  

@ol  

- @fa[poop] &rarr; Random Forests &rarr; EF
- @fa[poop] &rarr; Clustering &rarr; EF differs between clusters  
- @fa[poop] &rarr; Alpha-diversity &rarr; EF    

@olend

 





Note:

Species richness (OTU count)  "How many?"
How many different species could be detected in a microbial ecosystem?
Species richness is the number of different species in a sample. 
Practically, we count the number of distinguishable taxa (OTU's) in each sample   → QIIME OTU counts

Species diversity (Shannon index)  "How different?"
How are the microbes balanced to each other? Do we have species evenness (similar abundance level) or do some species dominate others?
Shannon index measures how evenly the microbes are distributed in a sample.



+++


## Societal and Scientific relevance  


  
@ul[](false)  
- promising target for intervention  
- translation to human studies  
- addressing shortcomings  
- methods development 
@ulend  
 


Note:
- laboratory setting clearly indicates importance
- this research needs to be translated to humans
- only one human study but using only one sample with a highly variable age: our study first study using multiple timepoints and both parental report and memory tests
- contributing to developing methods and visualization tool



---

## Methods


+++


## Participants 


@img[span-20](assets/img/bibo.jpg)

Note:

Question:  
How can I explain the missingness in the paper when I say we start with 192 mothers but then I only mention that we have sample size x that is different for all stool samples.

+++

@snap[midpoint]
## Measurements 
@snapend


@snap[north-west snap-pad-top span-33]
@box[bg-donders-two text-white  text-08](28 days#Fecal microbiota)
@snapend


@snap[north snap-pad-top span-33]
@box[bg-donders-three text-white  text-08](75 days#Fecal microbiota)
@snapend

@snap[north-east snap-pad-top span-33]
@box[bg-donders-four text-white text-08](105 days#Fecal microbiota)
@snapend


@snap[south-east snap-pad-bottom span-33]
@box[bg-donders-five text-white text-08](6 years#Fecal microbiota)
@snapend

@snap[south snap-pad-bottom span-33]
@box[bg-donders-six text-white text-08](8 years#BRIEF)
@snapend

@snap[south-west snap-pad-bottom span-33]
@box[bg-donders-seven text-white text-08](10 years#Digit Span & BRIEF)
@snapend



+++


## Statistical Analysis

- Extremely randomized trees
- K-means clustering
- Bayesian LM

Note:

EF:
- Tree ensemble method like random forest algorithm but:
  - uses whole training sample (reducing bias)
  - splitting the nodes with completely random cutoff points (reducing the variance)
  
- machine learning method for classification and regression
- robust to irrelevant variables, computational efficient, appropriate for high dimensional data, able to predict non-linear relationships




- EF: 
  1. Random 50/50 split
  2. Fit model
  3. predict scores from test set
  4. calculate Pearson 
  5. repeat 1000x

- Kmeans:Prediction Strength + Silhouette index



---

## Results


+++




## Extremely Randomized Trees

@img[span-50](assets/img/varimp-rf4.png)


+++


## Clustering



@img[span-55 revealborder](assets/img/clusterplot.png)




Note:
- no clustering in samples of first year
- clustering in the samples of 6 years
- no differences between cluster in cognitive outcome
- exploring subscales we found a difference in behavior regulation ($\mu_{2} - \mu_{1} = -3.45, \; 95\% \; CI \; [-6.56, \; -0.24]$)
- Behavior regulation at 8 years ($\mu_{2} - \mu_{1} = -3.19, \; 95\% \; CI \; [-6.40, \; 0.21]$)
- higher alpha diversity in cluster 2
- Cluster 1 is characterized by high relative abundance of bacteria belonging to Phylum Clostridium Cluster XIVa whereas cluster 2 is high in abundance of bacteria belonging to Bacteroidetes.

+++

@snap[north]
## Bayesian LM
@snapend

@snap[south-west span-50]
@img[](assets/img/shannonplots.png)
@snapend

@snap[south-east span-50]
@img[](assets/img/counterfactual_BR.png)
@snapend

---

## Discussion

- Bayesian GLM 2/20
- no Clustering
- Extremely Randomized Trees 2/20


Note:
- weak evidence
- laboratory settings
- clustering 
- future: functional level + diverse EF measures

---


@snap[mid]
#### Thank you for your attention!
@snapend

@snap[mid dtext text-07]
Questions?
@snapend

@snap[south-east second-logo-sized]
![](assets/img/dlogo.png) 
@snapend

@snap[south-west second-logo-sized]
![](assets/img/ruumc.png)
@snapend


+++

@snap[midpoint span-80]
@img[](assets/img/brief_example.png)
@snapend

+++


@snap[midpoint span-80]
@img[](https://upload.wikimedia.org/wikipedia/commons/a/a5/Biological_classification_L_Pengo_vflip.svg)
@snapend


+++

@snap[midpoint span-80]
@img[](assets/img/taxonomy.svg)
@snapend






