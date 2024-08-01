## Cognitive Diagnosis (CD)
### Research Directions

- **Prediction accuray:** It refers to developing and refining models to ensure they reliably forecast student performance and knowledge levels based on their responses and behavior.
   - Papers: [IRT](https://books.google.com.vn/books?hl=en&lr=&id=9Xm0AAAAQBAJ&oi=fnd&pg=PR1&dq=Susan%20E%20Embretson%20and%20Steven%20P%20Reise.%20Item%20response%20theory.%20Psychology%20Press,%202013.&ots=Ec6T_xMUYp&sig=uaOHLgo1b22uN_tUNtO6F6Y6h18&redir_esc=y), [MIRT](https://www.amazon.com/Multidimensional-Response-Statistics-Behavioral-Sciences/dp/0387899758), [CNCD-F](https://ieeexplore.ieee.org/document/9865139/)
   - Datasets: ASSISTment_2009-2010, FrcSub
- **Interpretability:** It focuses on making models understandable and transparent. This involves designing models that provide clear explanations for their predictions and decisions, enabling educators to gain insights into students' knowledge and learning processes, and facilitating the validation and effective use of the diagnostic results.  
   - Papers：[DINA](https://journals.sagepub.com/doi/10.3102/1076998607309474), [NCDM](https://ojs.aaai.org/index.php/AAAI/article/view/6080/5936), [KaNCD](https://ieeexplore.ieee.org/document/9865139/), [FuzzyCDF](https://dl.acm.org/doi/10.1145/3168361)
   - Datasets: ASSISTment_2009-2010, Math1, FrcSub
- **Data sparsity:** It focuses on addressing the challenges posed by sparse student interaction records or exercises with sparse knowledge components. Sparse data may lead to insufficient model training, reducing prediction accuracy and generalization. 
   - Papers: [NCDM+(CNCD-Q)](https://ojs.aaai.org/index.php/AAAI/article/view/6080/5936), [KSCD](https://dl.acm.org/doi/abs/10.1145/3511808.3557372), [DCD](https://proceedings.neurips.cc/paper_files/paper/2023/hash/3a14ae9951e8153a8fc814b5f506b5b7-Abstract-Conference.html)
   - Datasets: ASSISTment_2009-2010, Junyi, Eedi_2020
- **Group-level CD:** Estimating the cognitive levels of groups such as schools, classes, and study groups. By doing so, educators and administrators can identify strengths and weaknesses at a group level, allowing for targeted interventions and resource allocation.  
   - Papers: [MGCD](https://ieeexplore.ieee.org/document/9679064/), [HomoGCD](https://dl.acm.org/doi/abs/10.1145/3583780.3615287), [RGDT](https://ieeexplore.ieee.org/abstract/document/10388466)
   - Datasets: Eedi_2020, ASSISTment_2012-2013, SLP
- **Relation-aware:** It refers to understanding and leveraging the different relationships among students, exercises, and knowledge components. This means recognizing how students' knowledge states are influenced by their interactions with specific exercises and how these exercises relate to various knowledge components.  
   - Papers: [RCD](https://dl.acm.org/doi/10.1145/3404835.3462932), [HierCDF](https://dl.acm.org/doi/10.1145/3534678.3539486)
   - Datasets: ASSISTment_2009-2010, Junyi
- **Online CD:**  It refers to continuous assessment and updating of learners' knowledge states as data is collected in real-time. Unlike traditional methods that assume a stationary dataset, online CD deals with the dynamic nature of real-world scenarios where learner interactions, test items, and responses evolve over time.  
   - Papers: [ICD](https://dl.acm.org/doi/10.1145/3534678.3539399)
   - Datasets: ASSISTment_2009-2010
- **Dynamic CD:**  It combined with Knowledge Tracing focuses on modeling the evolving nature of students' knowledge states over time. This approach integrates the temporal dynamics of learning with sophisticated tracing techniques to provide a comprehensive view of students' cognitive development.  
   - Papers: [DNeuralCDM](https://ieeexplore.ieee.org/document/10065517)
   - Datasets: ASSISTment_2009-2010, ASSISTment_2012-2013, Bridge2Algebra_2006-2007
- **Long-tailed:**  It describes a scenario where a large number of occurrences or data points are concentrated at the tail end of a distribution. Understanding and managing these long-tailed distributions is crucial for effective cognitive diagnosis.  
   - Papers: [SCD](https://ojs.aaai.org/index.php/AAAI/article/view/25082/24854), [EIRS](https://www.ijcai.org/proceedings/2023/266)
   - Datasets: ASSISTment_2009-2010, Junyi
- **Cold-start:**  It refers to situations where there is little or no historical data available to inform the diagnostic process. This lack of prior data can significantly impact the ability to accurately assess and model students' knowledge states, especially at the beginning of a new learning or testing scenario.  
   - Papers: [BETA-CD](https://ojs.aaai.org/index.php/AAAI/article/view/25629), [TechCD](https://dl.acm.org/doi/10.1145/3539618.3591774), [DZCD](https://arxiv.org/abs/2312.13434), [ICDM](https://arxiv.org/abs/2404.11290)
   - Datasets: ASSISTment_2017, Junyi, FrcSub
- **Identifiability:**  It refers to the capability of diagnostic models to accurately distinguish between learners based on their different response data distributions. This means that the model should be able to differentiate learners’ knowledge states effectively, even when their response patterns vary significantly.  
   - Papers: [ID-CDF](https://arxiv.org/abs/2309.00300)
   - Datasets: ASSISTment_2009-2010, Algebera_2006-2007,Math1, Math2
- **Fairness:** It  pertains to ensuring that various sensitive attributes do not unduly influence the diagnosis of students. This involves making sure that diagnostic models provide equitable assessments and evaluations, regardless of factors such as race, gender, socioeconomic status, or other sensitive characteristics.  
   - Papers: [FairCD](https://www.sciengine.com/SCIS/doi/10.1007/s11432-022-3852-0;JSESSIONID=70b510e0-ae16-46ad-b44c-002e9792b9a1), [FairLISA](https://openreview.net/pdf?id=uFpjPJMkv6)
   - Datasets: PISA 2015
- **Uncertainty:** It refers to the model's confidence in its own predictions. It represents how sure or unsure the model is about its diagnostic results and can impact the reliability of these results.  
   - Papers: [UCD](http://arxiv.org/abs/2403.14676)
   - Datasets: FrcSub, Eedi
### Models
| Name | Publish | Year | Data | Technique | Research Directions |
| --- | --- | --- | --- | --- | --- |
| [IRT](https://books.google.com.vn/books?hl=en&lr=&id=9Xm0AAAAQBAJ&oi=fnd&pg=PR1&dq=Susan%20E%20Embretson%20and%20Steven%20P%20Reise.%20Item%20response%20theory.%20Psychology%20Press,%202013.&ots=Ec6T_xMUYp&sig=uaOHLgo1b22uN_tUNtO6F6Y6h18&redir_esc=y) | - | 1960 | Interaction | IRT | Prediction accuracy |
| [MIRT](https://www.amazon.com/Multidimensional-Response-Statistics-Behavioral-Sciences/dp/0387899758) | - | 1982 | Interaction | IRT | Prediction accuracy |
| [DINA](https://journals.sagepub.com/doi/10.3102/1076998607309474) | JEBS | 2009 | Interaction, Q-matrix | - | Interpretability |
| [FuzzyCDF](https://dl.acm.org/doi/10.1145/3168361) | TIST | 2018 | Interaction, Q-matrix | Fuzzy theory | Interpretability |
| [DIRT](https://dl.acm.org/doi/10.1145/3357384.3358070) | CIKM | 2019 | Interaction, Q-matrix, Exercise Texts | IRT, MLP, LSTM | interpretability |
| [NCDM](https://ojs.aaai.org/index.php/AAAI/article/view/6080/5936) | AAAI | 2020 | Interaction, Q-matrix | MLP, IRT | Interpretability |
| [NCDM+(CNCD-Q)](https://ojs.aaai.org/index.php/AAAI/article/view/6080/5936) | AAAI | 2020 | Interaction, Q-matrix | NCDM, CNN | Data sparsity |
| [CDGK](https://dl.acm.org/doi/abs/10.1145/3459637.3482311) | CIKM | 2021 | Interaction, Q-matrix | MLP, IRT | Interpretability |
| [ECD](https://dl.acm.org/doi/abs/10.1145/3447548.3467264) | KDD | 2021 | Interaction, Q-matrix, Student Features | Hierarchical Attention | Prediction accuracy |
| [MGCD](https://ieeexplore.ieee.org/document/9679064/) | ICDM | 2021 | Interaction, Q-matrix, Student Features | Attention | Group-level CD |
| [RCD](https://dl.acm.org/doi/10.1145/3404835.3462932) | SIGIR | 2021 | Interaction, Q-matrix, KC Prerequisite Relationships | Graph Neural Network | Relation-aware |
| [IRR](https://www.ijcai.org/proceedings/2021/241) | IJCAI | 2021 | Interaction, Q-matrix | Pairwise learning | Interpretability |
| [ICD](https://dl.acm.org/doi/10.1145/3534678.3539399) | KDD | 2022 | Interaction, Q-matrix | DTN | Online CD |
| [HierCDF](https://dl.acm.org/doi/10.1145/3534678.3539486) | KDD | 2022 | Interaction, Q-matrix, KC Prerequisite Relationships | Bayesian Network | Relation-aware |
| [CNCD-F](https://ieeexplore.ieee.org/document/9865139/) | TKDE | 2022 | Interaction, Q-matrix, Exercise Texts | TextCNN, NCDM | Prediction accuracy |
| [KaNCD](https://ieeexplore.ieee.org/document/9865139/) | TKDE | 2022 | Interaction, Q-matrix | NCDM | Interpretability |
| [ICD](https://www.sciencedirect.com/science/article/abs/pii/S0957417422023272) | ESWA | 2022 | Interaction, Q-matrix | MLP | Interpretability |
| [KSCD](https://dl.acm.org/doi/abs/10.1145/3511808.3557372) | CIKM | 2022 | Interaction, Q-matrix | NCDM | Data sparsity |
| [CDMFKC](https://dl.acm.org/doi/10.1145/3511808.3557096) | CIKM | 2022 | Interaction, Q-matrix | NCDM | Interpretability |
| [DNeuralCDM](https://ieeexplore.ieee.org/document/10065517) | TLT | 2023 | Interaction, Q-matrix | IRT, NCDM，GRU | Dynamic CD |
| [MvCRF](https://ieeexplore.ieee.org/abstract/document/10210482) | TKDE | 2023 | Interaction, Q-matrix | Effort trait, Compensation mechanism, | Interpretability |
| [FairCD](https://www.sciengine.com/SCIS/doi/10.1007/s11432-022-3852-0;JSESSIONID=70b510e0-ae16-46ad-b44c-002e9792b9a1) | SCIS | 2023 | Interaction, Q-matrix, Student Features | Disentanglement, Adversarial | Fairness |
| [FairLISA](https://openreview.net/pdf?id=uFpjPJMkv6) | NeurIPS | 2023 | Interaction, Q-matrix, Student Features | Adversarial | Fairness |
| [DCD](https://proceedings.neurips.cc/paper_files/paper/2023/hash/3a14ae9951e8153a8fc814b5f506b5b7-Abstract-Conference.html) | NeurIPS | 2023 | Interaction, Q-matrix, KC Inclusion Relationships | Disentanglement, VAE | Data sparsity |
| [HomoGCD](https://dl.acm.org/doi/abs/10.1145/3583780.3615287) | CIKM | 2023 | Interaction, Q-matrix | MLP | Group-level CD |
| [DAISim](https://dl.acm.org/doi/abs/10.1145/3583780.3615060) | CIKM | 2023 | Interaction, Q-matrix | Adversarial | Prediction accuracy |
| [GLNC](https://www.sciencedirect.com/science/article/abs/pii/S0957417423021395) | ESWA | 2023 | Interaction, Q-matrix | Attention, MLP | Prediction accuracy |
| [SCD](https://ojs.aaai.org/index.php/AAAI/article/view/25082/24854) | AAAI | 2023 | Interaction, Q-matrix | GCN | Long-tailed |
| [BETA-CD](https://ojs.aaai.org/index.php/AAAI/article/view/25629) | AAAI | 2023 | Interaction, Q-matrix | Meta learning | Cold-start |
| [EIRS](https://www.ijcai.org/proceedings/2023/266) | IJCAI | 2023 | Interaction, Q-matrix | Partial-Order Response Sampling | Long-tailed |
| [CBICDM](https://link.springer.com/chapter/10.1007/978-981-99-8067-3_16) | ICONIP | 2023 | Interaction, Q-matrix | Bayesian network | Interpretability |
| [TechCD](https://dl.acm.org/doi/10.1145/3539618.3591774) | SIGIR | 2023 | Interaction, Q-matrix | GCN | Cold-start |
| [QCCDM](https://github.com/lswhim/CDM_ILOG) | ECAI | 2023 | Interaction, Q-matrix | Structure Causal Model | Data sparsity |
| [RGDT](https://ieeexplore.ieee.org/abstract/document/10388466) | TKDE | 2024 | Interaction, Q-matrix, Student Features | Dual-side graph transformers | Group-level CD |
| [DZCD](https://arxiv.org/abs/2312.13434) | AAAI | 2024 | Interaction, Q-matrix | Disentanglement | Cold-start |
| [CMES](https://arxiv.org/abs/2312.10110) | AAAI | 2024 | Interaction, Q-matrix | Attention, Sampling | Data sparsity |
| [ACD](https://ojs.aaai.org/index.php/AAAI/article/view/27818) | AAAI | 2024 | Interaction, Q-matrix, Student Features | Contrastive learning | Prediction accuracy |
| [ICDM](https://arxiv.org/abs/2404.11290) | WWW | 2024 | Interaction, Q-matrix | GCN | Cold-start |
| [ID-CDF](https://arxiv.org/abs/2309.00300) | WWW | 2024 | Interaction, Q-matrix | Inductive learning | Identifiability and Interpretability |
| [UCD](http://arxiv.org/abs/2403.14676) | WWW | 2024 | Interaction, Q-matrix | Bayesian Variational Inference | Uncertainty |
| [ASG-CD](http://arxiv.org/abs/2403.05559) | Arxiv | 2024 | Interaction, Q-matrix | GNN | Prediction accuracy |
| [DisKCD](https://arxiv.org/abs/2405.16003) | Arxiv | 2024 | Interaction, Q-matrix, Exercise texts, Course slides | Attention, MLP | Data sparsity |


## Knowledge Tracing (KT)
### Research Directions

- **Prediction accuracy:** It refers to the model’s ability to correctly forecast students' future performance based on their past interactions and knowledge states. It measures how well the model can predict which questions or exercises a student is likely to answer correctly or incorrectly.  
   - Papers: [BKT](https://link.springer.com/article/10.1007/BF01099821), [DKT](https://proceedings.neurips.cc/paper_files/paper/2015/hash/bac9162b47c56fc8a4d2a519803d51b3-Abstract.html), [DKVMN](https://arxiv.org/pdf/1611.08108.pdf)
   - Datasets: Simulated-5, ASSISTment_2009-2010, ASSISTment_2015-2016, Statics - Fall 2011
- **Interpretability:** It involves understanding and explaining the reasoning behind the model’s predictions. It focuses on making the model's decision-making process transparent and understandable to educators and stakeholders.  
   - Papers: [KPT](https://dl.acm.org/doi/10.1145/3132847.3132929), [Deep-IRT](https://arxiv.org/abs/1904.11738), [KQN](https://dl.acm.org/doi/abs/10.1145/3303772.3303786), [EKT](https://ieeexplore.ieee.org/document/8744302)
   - Datasets: Math1, Math2, ASSISTment_2009-2010, ASSISTment_2015-2016, Statics - Fall 2011
- **Cold-start:** It refers to situations where there is little or no historical data available for new students, exercises, or knowledge components. This lack of data can hinder the model’s ability to make accurate predictions.  
   - Papers: [EERNN](https://ojs.aaai.org/index.php/AAAI/article/view/11864), [EKT](https://ieeexplore.ieee.org/document/8744302), [QDCKT](https://dl.acm.org/doi/abs/10.1145/3589334.3645582)
   - Datasets: ASSISTment_2009-2010, ASSISTment_2017, Algebera_2005-2006, Algebera_2006-2007
- **Data sparsity:** It refers to situations where student interaction records are sparse or where exercises cover only a limited set of knowledge components. Sparse data can result in incomplete or insufficient information for accurate model training and evaluation.  
   - Papers: [SAKT](https://experts.umn.edu/en/publications/a-self-attentive-model-for-knowledge-tracing), [qDKT](https://people.umass.edu/~andrewlan/papers/20edm-qdkt.pdf), [LPKT](http://staff.ustc.edu.cn/~qiliuql/files/Publications/Shuanghong-Sheng-KDD21.pdf), [CMKT](https://ieeexplore.ieee.org/abstract/document/9850398/), [CMVF](https://arxiv.org/abs/2309.01179), [QRCL](https://www.sciencedirect.com/science/article/pii/S0020025523016183)
   - Datasets: Simulated-5, ASSISTment_2009-2010, ASSISTment_2015-2016, Statics - Fall 2011, EdNet-KT1
- **Forget:** It  refers to the phenomenon where a student's retention of learned material decreases over time. The more frequently students engage with and practice a particular knowledge component, the more they are likely to retain that knowledge and less likely to forget it.  
   - Papers: [DKTForget](https://dl.acm.org/doi/10.1145/3308558.3313565), [FoLiBi](https://dl.acm.org/doi/abs/10.1145/3583780.3615191), [CPF](http://arxiv.org/abs/2404.12127)
   - Datasets: ASSISTment_2009-2010, ASSISTment_2012-2013, Algebera_2006-2007, Bridge2Algebra_2006-2007
- **Relation-aware:** It considers the various relationships among students, exercises, and knowledge components. It involves understanding how these entities interact and influence each other, such as how students' knowledge of certain components affects their performance on related exercises.  
   - Papers: [RKT](https://arxiv.org/pdf/2008.12736.pdf), [SKT](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9338285), [GIKT](https://link.springer.com/chapter/10.1007/978-3-030-67658-2_18), [PEBG](https://arxiv.org/pdf/2012.05031.pdf), [HGKT](https://dl.acm.org/doi/abs/10.1145/3477495.3532004)
   - Datasets: ASSISTment_2012-2013, Junyi, Statics - Fall 2011
- **Cross-effects:** They refer to the influence of a student's previous interactions with both the same knowledge component and other knowledge components on their current mastery of a particular knowledge component. 
   - Papers:[HawkesKT](https://dl.acm.org/doi/10.1145/3437963.3441802)
   - Datasets: ASSISTment_2009-2010, ASSISTment_2012-2013
- **Long sequences:** It refers to the continuous and extended learning experiences that students undergo in real-world educational systems. This results in sequences of interactions with varying lengths, as students engage with a wide range of exercises and knowledge components over time.  
   - Papers: [CPKT](https://dl.acm.org/doi/abs/10.1145/3583780.3614822)
   - Datasets: EdNet, ASSISTment_2015-2016, Junyi
- **Answer bias:** It refers to the imbalanced distribution of correct and incorrect answers for each question. This means that some questions might receive predominantly correct or incorrect responses, leading to skewed data.  
   - Papers: [CORE](https://arxiv.org/abs/2308.07779)
   - Datasets: ASSISTment_2009-2010, ASSISTment_2017, EdNet
- **Skill Switching Phenomenon:** It  describes the irregular switching of latent skills when learners respond to exercises in an e-learning system. This means that learners' underlying skills can change unpredictably based on their interactions with different exercises.  
   - Papers: [DLKT](https://dl.acm.org/doi/abs/10.1145/3589340)
   - Datasets: ASSISTment_2009-2010, ASSISTment_2017, Statics - Fall 2011
- **Stable KT:** It refers to the approach of tracing a learner's knowledge evolution over time, rather than merely predicting response patterns and inferring knowledge states based on observed data.  
   - Papers: [DTransformer](https://yxonic.github.io/pdfs/yin2023tracing.pdf)
   - Datasets: ASSISTment_2009-2010, ASSISTment_2017, Algebera_2005-2006, Statics - Fall 2011
- **Anomaly detection:** It involves identifying conflicting or inconsistent responses from a student for the same exercise within a short period, which is likely indicative of data noise rather than genuine changes in knowledge.  
   - Papers: [HD-KT](https://dl.acm.org/doi/abs/10.1145/3589334.3645718)
   - Datasets: ASSISTment_2012-2013, ASSISTment_2017, Junyi
- **Low-resource:** It refers to the challenge of working with educational datasets for knowledge tracing that often have limited student learning records. This limitation arises from the scarcity of data collected on student interactions, which can hinder the development and performance of KT models.  
   - Papers: [LoReKT](http://arxiv.org/abs/2403.06725)
   - Datasets: ASSISTment_2009-2010, Eedi_2020, Bridge2Algebra_2006-2007,  EdNet
- **Student behavior:** It involves incorporating personalized behavioral information, such as emotions, into the knowledge tracing model. This means taking into account how individual students' behaviors can impact their learning and performance.  
   - Papers: [T-DEKT](https://arxiv.org/abs/2405.16799)
   - Datasets: ASSISTment_2012-2013, EdNet
- **Efficiency:** It refers to the model training and inference process's speed and resource utilization, including constraints related to computational and storage resources. Efficient models can be trained and deployed with minimal resource consumption while maintaining high performance.  
   - Papers: [Mamba4KT](https://arxiv.org/abs/2405.16542)
   - Datasets: ASSISTment_2012-2013, ASSISTment_2017, Eedi_2020
### Models
| Name | Publish | Year | Data | Technique | Research Directions |
| --- | --- | --- | --- | --- | --- |
| [BKT](https://link.springer.com/article/10.1007/BF01099821) | UMUAI | 1994 | Interaction,Q-matrix | Bayesian network | Prediction accuracy |
| [LFA](https://link.springer.com/chapter/10.1007/11774303_17) | ICITS | 2006 | Interaction,Q-matrix | Logistic Regression | Prediction accuracy |
| [AFM](https://dl.acm.org/doi/10.1007/978-3-540-69132-7_111) | ITS | 2008 | Interaction,Q-matrix | Logistic Regression | Prediction accuracy |
| [PFA](https://dl.acm.org/doi/10.5555/1659450.1659529) | AIED | 2009 | Interaction,Q-matrix | Logistic Regression | Prediction accuracy |
| [DKT](https://proceedings.neurips.cc/paper_files/paper/2015/hash/bac9162b47c56fc8a4d2a519803d51b3-Abstract.html) | NIPS | 2015 | Interaction | RNN/LSTM | Prediction accuracy |
| [HIRT, TIRT](https://www.educationaldatamining.org/EDM2016/proceedings/paper_145.pdf) | EDM | 2016 | Interaction | IRT | Prediction accuracy |
| [DBKT/DBN](https://dl.acm.org/doi/10.1109/TLT.2017.2689017) | TLT | 2017 | Interaction,Q-matrix | DBN | Prediction accuracy |
| [DKVMN](https://arxiv.org/pdf/1611.08108.pdf) | WWW | 2017 | Interaction | MANN | Prediction accuracy |
| [KPT](https://dl.acm.org/doi/10.1145/3132847.3132929) | CIKM | 2017 | Interaction,Q-matrix | Probabilistic Modeling | Interpretability |
| [DKT+](https://arxiv.org/pdf/1806.02180.pdf) | L@S | 2018 | Interaction | RNN/LSTM | Prediction accuracy |
| [DKT_DSC](https://ieeexplore.ieee.org/abstract/document/8594965) | ICDM | 2018 | Interaction | RNN/LSTM | Prediction accuracy |
| [P-DKTC](https://ieeexplore.ieee.org/abstract/document/8594828) | ICDM | 2018 | Interaction, Q-matrix, KC Prerequisite Relationships | DKT | Prediction accuracy |
| [EERNN](https://ojs.aaai.org/index.php/AAAI/article/view/11864) | AAAI | 2018 | Interaction, Exercise texts | LSTM, Attention | Cold-start |
| [KTM](https://arxiv.org/abs/1811.03388) | AAAI | 2019 | Interaction, Q-matrix | Factorization machines | Prediction accuracy |
| [Deep-IRT](https://arxiv.org/abs/1904.11738) | EDM | 2019 | Interaction | Memory, IRT | Interpretability |
| [SAKT](https://experts.umn.edu/en/publications/a-self-attentive-model-for-knowledge-tracing) | EDM | 2019 | Interaction | Attention | Data sparsity |
| [KQN](https://dl.acm.org/doi/abs/10.1145/3303772.3303786) | LAK | 2019 | Interaction, Q-matrix | RNN, MLP | Interpretability |
| [DKTForget](https://dl.acm.org/doi/10.1145/3308558.3313565) | WWW | 2019 | Interaction, Q-matrix | RNN/LSTM | Forget |
| [SKVMN](https://dl.acm.org/doi/10.1145/3331184.3331195) | SIGIR | 2019 | Interaction | Memory | Prediction accuracy |
| [GKT](https://dl.acm.org/doi/abs/10.1145/3350546.3352513) | WI | 2019 | Interaction | GNN | Prediction accuracy |
| [EKT](https://ieeexplore.ieee.org/document/8744302) | TKDE | 2019 | Interaction, Q-matrix, Exercise Texts | LSTM, Attention, Memory | Cold-start, Interpretability |
| [qDKT](https://people.umass.edu/~andrewlan/papers/20edm-qdkt.pdf) | EDM | 2020 | Interaction | RNN/LSTM | Data sparsity |
| [KTM-DLF](https://link.springer.com/article/10.1007/s10489-020-01756-7) | APIN | 2020 | Interaction, Q-matrix | Factorization machines | Prediction accuracy |
| [AKT](https://dl.acm.org/doi/abs/10.1145/3394486.3403282) | KDD | 2020 | Interaction, Q-matrix | Attention | Interpretability |
| [CKT](https://dl.acm.org/doi/abs/10.1145/3397271.3401288) | SIGIR | 2020 | Interaction | CNN | Prediction accuracy |
| [RKT](https://arxiv.org/pdf/2008.12736.pdf) | CIKM | 2020 | Interaction, Exercise Relation Graph | Attention | Relation-aware |
| [SAINT](https://dl.acm.org/doi/10.1145/3386527.3405945) | L@S | 2020 | Interaction, Exercise Features | Attention, Transformer | Prediction accuracy |
| [SKT](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9338285) | ICDM | 2020 | Interaction, Q-matrix, KC Prerequisite Relationships | RNN | Relation-aware |
| [GIKT](https://link.springer.com/chapter/10.1007/978-3-030-67658-2_18) | ECML PKDD | 2020 | Interaction, Q-matrix | GCN, RNN | Relation-aware |
| [PEBG](https://arxiv.org/pdf/2012.05031.pdf) | IJCAI | 2020 | Interaction, Q-matrix | Bipartite Graph | Relation-aware |
| [IEKT](https://dl.acm.org/doi/10.1145/3404835.3462827) | SIGIR | 2021 | Interaction | RNN | Prediction accuracy |
| [FDKT](https://dl.acm.org/doi/abs/10.1145/3437963.3441747) | WSDM | 2021 | Interaction, Q-matrix, Student Features | Federated learning | Prediction accuracy |
| [HawkesKT](https://dl.acm.org/doi/10.1145/3437963.3441802) | WSDM | 2021 | Interaction, Q-matrix | Hawkes Process | Cross-effects |
| [TC-MIRT](https://www.sciencedirect.com/science/article/pii/S0950705121000824) | KBS | 2021 | Interaction, Q-matrix | RNN, MIRT | Interpretability |
| [SAINT+](https://dl.acm.org/doi/10.1145/3448139.3448188) | LAK | 2021 | Interaction, Exercise Features | Attention,Transformer | Prediction accuracy |
| [MF_DAKT](https://dl.acm.org/doi/abs/10.1145/3459637.3482372) | CIKM | 2021 | Interaction | Dual-attentional | Prediction accuracy |
| [ATKT](https://arxiv.org/pdf/2108.04430.pdf) | ACM MM | 2021 | Interaction, Q-matrix | Attention, LSTM | Prediction accuracy |
| [LPKT](http://staff.ustc.edu.cn/~qiliuql/files/Publications/Shuanghong-Sheng-KDD21.pdf) | KDD | 2021 | Interaction, Q-matrix | GRU, MLP | - |
| [IKT](https://ojs.aaai.org/index.php/AAAI/article/view/21560) | AAAI | 2022 | Interaction, Q-matrix | Causal Relation, TAN | Interpretability |
| [AdaptKT](https://dl.acm.org/doi/10.1145/3488560.3498379) | WSDM | 2022 | Interaction | LSTM | - |
| [CoKT](https://dl.acm.org/doi/abs/10.1145/3488560.3498374) | WSDM | 2022 | Interaction, Q-matrix | GRU | Prediction accuracy |
| [CL4KT](https://dl.acm.org/doi/abs/10.1145/3485447.3512105) | WWW | 2022 | Interaction, Q-matrix | Transformer, Contrastive Learning | Prediction accuracy |
| [DIMKT](https://dl.acm.org/doi/abs/10.1145/3477495.3531939) | SIGIR | 2022 | Interaction, Q-matrix | Sequential Neural Network | Interpretability |
| [HGKT](https://dl.acm.org/doi/abs/10.1145/3477495.3532004) | SIGIR | 2022 | Interaction | HGNN, Attention | Relation-aware |
| [LFBKT](https://dl.acm.org/doi/abs/10.1145/3511808.3557622) | CIKM | 2022 | Interaction, Q-matrix | MLP | - |
| [CT-NCM](https://www.semanticscholar.org/paper/Reconciling-Cognitive-Modeling-with-Knowledge-A-Ma-Wang/d3b4115906be4939b7f93736090ec1844d9ae591) | IJCAI | 2022 | Interaction, Q-matrix | Hawkes Process, LSTM | - |
| [LPKT-S](https://ieeexplore.ieee.org/document/9950313) | TKDE | 2022 | Interaction, Q-matrix | GRU, MLP | - |
| [DGMN](https://arxiv.org/abs/2108.08105) | TKDE | 2022 | Interaction, Q-matrix | GCN, Attention Memory | Prediction accuracy |
| [CMKT](https://ieeexplore.ieee.org/abstract/document/9850398/) | TLT | 2022 | Interaction, Q-matrix | GRU, MLP | Data sparsity |
| [AGKT](https://zenodo.org/record/6853057) | EDM | 2022 | Interaction | HGNN | Prediction accuracy |
| [QIKT](https://arxiv.org/abs/2302.06885) | AAAI | 2023 | Interaction, Q-matrix | LSTM, IRT | Interpretability |
| [DAKTN](https://ojs.aaai.org/index.php/AAAI/article/view/26214) | AAAI | 2023 | Interaction | MLP, IRT | Prediction accuracy |
| [SFKT](https://dl.acm.org/doi/abs/10.1145/3583780.3614988) | CIKM | 2023 | Interaction, Q-matrix, Time interval | Attention, Contrastive learning | Prediction accuracy |
| [FoLiBi](https://dl.acm.org/doi/abs/10.1145/3583780.3615191) | CIKM | 2023 | Interaction | Attention, MLP | Forget |
| [CPKT](https://dl.acm.org/doi/abs/10.1145/3583780.3614822) | CIKM | 2023 | Interaction | Memory | Long sequences |
| [CMKT](https://dl.acm.org/doi/abs/10.1145/3583780.3614827) | CIKM | 2023 | Interaction, Q-matrix | MIRT,Counterfactual Monotonicity | Prediction accuracy |
| [CMVF](https://arxiv.org/abs/2309.01179) | ICDM | 2023 | Interaction, Q-matrix | Variational Inference | Data sparsity |
| [FKT](https://www.sciencedirect.com/science/article/pii/S095741742302609X) | ESWA | 2023 | Interaction, Q-matrix, Timestamp | Attention | Prediction accuracy |
| [TSKT](https://www.sciencedirect.com/science/article/pii/S0957417423027513) | ESWA | 2023 | Interaction, Q-matrix | GNN, LSTM | Prediction accuracy |
| [DKTMR](https://www.sciencedirect.com/science/article/pii/S0957417423030750) | ESWA | 2023 | Interaction, Q-matrix | GAN, GRU | Relation-aware |
| [QRCL](https://www.sciencedirect.com/science/article/pii/S0020025523016183) | ESWA | 2023 | Interaction, Q-matrix | SVD,GNN | Data sparsity |
| [ABQR](https://dl.acm.org/doi/abs/10.1145/3581783.3612044) | MM | 2023 | Interaction, Q-matrix | Adversarial | Prediction accuracy |
| [AAKT](https://www.techrxiv.org/doi/full/10.36227/techrxiv.24487747.v1) | TLT | 2023 | Interaction, Q-matrix, Response time | Transformer, MLP | Prediction accuracy |
| [OPKT](https://ieeexplore.ieee.org/abstract/document/10328390) | TLT | 2023 | Interaction, Q-matrix | Transformer | Data sparsity |
| [MVGKT](https://ieeexplore.ieee.org/abstract/document/10202591) | TLT | 2023 | Interaction, Q-matrix | GCN, GRU, Attention | Prediction accuracy |
| [MA-DKT](https://www.spiedigitallibrary.org/conference-proceedings-of-spie/12941/129412N/A-deep-knowledge-tracing-model-based-on-multi-head-self/10.1117/12.3011559.short#_=_) | AHPCAI | 2023 | Interaction, Q-matrix | LSTM, Attention | Prediction accuracy |
| [RCKT](https://arxiv.org/abs/2312.10045) | Arxiv | 2023 | Interaction | Counterfactual reasoning | Interpretability |
| [CORE](https://arxiv.org/abs/2308.07779) | Arxiv | 2023 | Interaction | Counterfactual reasoning | Answer bias |
| [BiCo](https://dl.acm.org/doi/abs/10.1145/3638055) | TKDD | 2023 | Interaction, Q-matrix, Exercise Texts | Contrastive learning | Prediction accuracy |
| [DLKT](https://dl.acm.org/doi/abs/10.1145/3589340) | TOIS | 2023 | Interaction, Q-matrix | MAN | Skill Switching Phenomenon |
| [MRT-KT](https://dl.acm.org/doi/10.1145/3580595) | TOIS | 2023 | Interaction, Q-matrix, Timestamp | Transformer | Relation-aware |
| [SimpleKT](https://arxiv.org/abs/2302.06881) | ICLR | 2023 | Interaction, Q-matrix | Attention | Prediction accuracy |
| [DTransformer](https://yxonic.github.io/pdfs/yin2023tracing.pdf) | WWW | 2023 | Interaction, Q-matrix | Transformer, Contrastive Learning | Stable KT |
| [MAKT](https://link.springer.com/article/10.1007/s11280-023-01190-y) | WWW | 2023 | Interaction, Q-matrix, Timestamp,  Student features | Attention | Prediction accuracy |
| [LBKT](http://staff.ustc.edu.cn/~huangzhy/files/papers/BihanXu-KDD2023.pdf) | KDD | 2023 | Interaction, Q-matrix, Timestamp,  Student features | MLP | Prediction accuracy |
| [ENAS-KT](https://arxiv.org/abs/2310.01180) | NeurIPS | 2023 | Interaction, Q-matrix, Timestamp, Exercise features | Neural Architecture Search | Prediction accuracy |
| [GraphCA](https://ieeexplore.ieee.org/abstract/document/10266657) | IEEE/CAA | 2023 | Interaction, Q-matrix | Counterfactual representation, GNN, Contrastive learning | Data sparsity,Relation-aware |
| [QDCKT](https://dl.acm.org/doi/abs/10.1145/3589334.3645582) | WWW | 2024 | Interaction, Q-matrix | LSTM, MLP | Cold-start |
| [MIKT](https://dl.acm.org/doi/abs/10.1145/3589334.3645373) | WWW | 2024 | Interaction, Q-matrix | IRT, MLP | Interpretability |
| [HD-KT](https://dl.acm.org/doi/abs/10.1145/3589334.3645718) | WWW | 2024 | Interaction, Q-matrix, Timestamp | LSTM, GNN, Attention | Anomaly detection |
| [SYNSAINT](https://d197for5662m48.cloudfront.net/documents/publicationstatus/207325/preprint_pdf/c2a95dfc700af81fb4e0c819a8541700.pdf) | TLT | 2024 | Interaction, Q-matrix, Timestamp | Multi-head Attention, MLP | Prediction accuracy |
| [CoSKT](https://ieeexplore.ieee.org/document/10495188/) | TLT | 2024 | Interaction, Q-matrix | Self-attention, LSTM, Self-supervised learning | Prediction accuracy |
| [HyperKT](https://ieeexplore.ieee.org/document/10506993) | TNNLS | 2024 | Interaction | Contrastive learning, Hyperedge distillation, Hypergraph learning | Prediction accuracy |
| [GSKPM](https://epubs.siam.org/doi/10.1137/1.9781611978032.43) | SDM | 2024 | Interaction, KC relations | GNN, HGNN, LSTM | Cold-start |
| [CPF](http://arxiv.org/abs/2404.12127) | SCIS | 2024 | Interaction, Q-matrix, KC Prerequisite Relationships, Time | MLP | Forget |
| [FDKT](https://dl.acm.org/doi/10.1145/3656167) | TOIS | 2024 | Interaction, Q-matrix,Timestamp | Fuzzy reasoning | Interpretability |
| [PSKT](https://openreview.net/forum?id=gDXAv76iP2) | MM | 2024 | Interaction, Q-matrix,Timestamp | Sequential Neural Network, IRT | Interpretability |
| [LoReKT](http://arxiv.org/abs/2403.06725) | Arxiv | 2024 | Interaction, Q-matrix | Multi-head Attention, MLP | Low-resource |
| [T-DEKT](https://arxiv.org/abs/2405.16799) | Arxiv | 2024 | Interaction, Q-matrix, Student features, Time | MLP | Student behavior |
| [Mamba4KT](https://arxiv.org/abs/2405.16542) | Arxiv | 2024 | Interaction, Q-matrix | Mamba,Rasch model | Efficiency |

