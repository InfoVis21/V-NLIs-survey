# A Survey of Natural Language Interfaces for Data Visualization
This repository provides supplementary materials for our paper titled **A Survey of Natural Language Interfaces for Data Visualization**. 

Utilizing Visualization-oriented Natural Language Interfaces (V-NLIs) as a complementary input modality to direct manipulation for visual analytics can provide an engaging user experience. It allows users to only focus on the questions about data, rather than how to operate the interface to visualization tools. However, designing practical V-NLIs is a challenging task due to the complex and ambiguous nature of human language, the difficulty of maintaining context in conversational flow, the hardness to tell fascinating data stories, and lack of discoverability. In the past two decades, leveraging advanced natural language processing technologies, various V-NLIs have been developed both within academic research and commercial software, especially in recent years. In our paper, we conducted a comprehensive review of the existing V-NLIs. Based on the field challenge type they deal with, we sorted out related works and analyzed their characteristics. In addition, we designed a set of test cases for V-NLIs and evaluated four state-of-the-art systems to examine whether we are ready to ask our data freely, along with discovering problems not found yet. Finally, we shed light on several promising directions for future work in the community.

The materials include:

|                          | Description                                                                                                                   | File                                    |
|--------------------------|-------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------|
| Survey                   | Survey of related works.                                                                                                      | ```./Survey.xlsx```                     |
| Dataset                  | Dataset for evluating existing V-NLIs.                                                                                        | ```./Dataset/*.csv```                   |
| Test cases and results   | Test cases and judged evaluation results.                                                                                     | ```./Test_cases_and_results.xlsx```     |
| Evaluation_visualization | Visualizations generated in the evaluation, files are named as task_system_query type.png such as Cluster_NL4DV_specific.png. | ```./Evaluation vis/*.png``` |


## Available Datasets for V-NLIs
---

* [NLV](https://nlvcorpus.github.io/)

There is a lack of empirical understanding of how people specify visualizations through natural language. Researchers of NLV conducted an online study (N = 102), showing participants a series of visualizations and asking them to provide utterances they would pose to generate the displayed charts. From the responses, they curated a dataset of 893 utterances and characterized the utterances according to (1) their phrasing (e.g., commands, queries, questions) and (2) the information they contained (e.g., chart types, data aggregations). 

* [Quda](https://freenli.github.io/quda/)

Quda aims to help V-NLIs recognize analytic tasks from free-form natural language by training and evaluating cutting-edge multi-label classification models. The dataset contains 14035 diverse user queries, and each is annotated with one or multiple analytic tasks. Quda achieves this goal by first gathering seed queries with data analysts and then employing extensive crowd force for paraphrase generation and validation. This work is the first attempt to construct a large-scale corpus for recognizing analytic tasks.

* [VisQA](https://github.com/dhkim16/VisQA-release)

People often use charts to analyze data, answer questions and explain their answers to others. In a formative study, Kim et al. found that such human-generated questions and explanations commonly refer to visual features of charts. Based on this study, they developed an automatic chart question answering pipeline that generates
visual explanations describing how the answer was obtained. During the study, they showed people various bar charts and line charts, and collected questions participants posed about the charts along with their answers and explanations to those questions.