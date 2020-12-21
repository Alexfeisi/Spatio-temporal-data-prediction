# Spatio-temporal-data-prediction
 与时空数据预测相关的论文及代码


This project includes: papers of the top conferences/journals in the field of Spatio-Temporal domain, relevant data sets and information of well-known experts and scholars in the field of Spatio-Temporal domain.

# Contribution

Contributions are always welcome! Make an individual pull request for each suggestion. Please follow the specification：**[contribute](./contribute.md)**.

# Content

<table>
<tr><td colspan="2"><a href="#survey-papers">1. Survey</a></td></tr> 
<tr><td colspan="2"><a href="#applications">2. Applications</a></td></tr> 
<tr>
    <td>&emsp;<a href="#traffic-prediction">2.1 Traffic Prediction</a></td>
    <td>&ensp;<a href="#flow-prediction">2.2 Flow Prediction</a></td>
</tr> 
<tr>
    <td>&emsp;<a href="#demand-prediction">2.3 Demand Prediction</a></td>
    <td>&ensp;<a href="#travel-time-or-arrive-time-prediction">2.4 Travel time or Arrive time Prediction</a></td>
</tr>
<tr>
	<td>&emsp;<a href="#speed-prediction">2.5 Speed Prediction</a></td>
    <td>&ensp;<a href=""> </a></td>    
</tr>
<tr><td colspan="2"><a href="#datasets">3. Datasets</a></td></tr>
<tr>
    <td>&emsp;<a href="#sensor-data">3.1 Sensor data</a></td>
    <td>&ensp;<a href="#trajectory-data">3.2 Trajectory data</a></td>
</tr> 
<tr>
    <td>&emsp;<a href="#Others">3.3 others</a></td>
</tr> 
<tr><td colspan="2"><a href="#experts">4. Experts</a></td></tr> 
</table>



# Survey papers

[1] **Urban Computing: Concepts, Methodologies, and Applications.** ACM Transactions on Intelligent Systems and Technology 2014. [paper](https://www.microsoft.com/en-us/research/wp-content/uploads/2016/02/UrbanComputing-zheng-tist2014.pdf)

*YU ZHENG, LICIA CAPRA, OURI WOLFSON, HAI YANG*

---

[2] **Deep Learning for Spatio-Temporal Data Mining: A Survey.** IEEE Transactions on Knowledge and Data Engineering(TKDE) 2020. [paper](https://arxiv.org/pdf/1906.04928.pdf)

*Senzhang Wang, Jiannong Cao, Fellow, Philip S. Yu*

---

[3] **A Survey on Modern Deep Neural Network for Traffic Prediction: Trends, Methods and Challenges.** IEEE Transactions on Knowledge and Data Engineering(TKDE) 2020. [paper](https://ieeexplore.ieee.org/abstract/document/9112608)

*David Alexander Tedjopurnomo, Zhifeng Bao, Baihua Zheng, Farhana Murtaza Choudhury, Kai Qin*

---

[4] **How to Build a Graph-Based Deep Learning Architecture in Traffic Domain: A Survey.** arXiv 2020. [paper](https://arxiv.org/pdf/2005.11691.pdf)

*Jiexia Ye, Juanjuan Zhao, Kejiang Ye, Chengzhong Xu*

---

# Applications

## [Traffic Prediction](#content)

本节为交通预测主题相关文章，即文中未指明特定研究主题（如速度/流量预测等），且实验部分也使用多类数据集验证的文章。

This section is for traffic prediction topic-related articles, which refers to a category of articles that do not specify a specific research topic (e.g., speed/traffic prediction, etc.) and where the experimental part is also validated using multiple types of datasets.

<details><summary> 2020 </summary>


[1] **[Spatio-Temporal Graph Structure Learning for Traffic Forecasting.](./papers/2020/AAAI/SLC/SLC)** AAAI 2020. [note](./papers/2020/AAAI/SLC/note.md)

| Models |  Modules   |                 Architecture                 | conclusion                                                   |
| :----- | :--------: | :------------------------------------------: | :----------------------------------------------------------- |
| SLC    | SLCNN, P3D | ![STGCN](./papers/2020/AAAI/SLC/img/SLC.png) | This paper proposes a new type of graph convolution formula. **The article mentions that it is necessary to learn not only the feature information on the graph, but also the structure information of the graph**, which means that the structure of the graph changes dynamically. Use P3D to model the time dependence. |

*[Q Zhang](https://scholar.google.com.hk/citations?user=RDwnNsQAAAAJ&hl=zh-CN&oi=sra), J Chang, [G Meng](https://scholar.google.com.hk/citations?user=5hti_r0AAAAJ&hl=zh-CN&oi=sra), [S Xiang](https://scholar.google.com.hk/citations?user=0ggsACEAAAAJ&hl=zh-CN&oi=sra), C Pan*

------

</details>


## [Flow Prediction](#content)

<details><summary> 2020 </summary>
[1] **[Deep Learning Architecture for Short-TermPassenger Flow Forecasting inUrban Rail Transit](./ResNet-LSTM-GCN)** IEEE 2020. [note](./ResNet-LSTM-GCN/README.md). 


| Models | Modules |                         Architecture                         | Highlights                                                   |
| :----: | :-----: | :----------------------------------------------------------: | :----------------------------------------------------------- |
| ResLSTM  |         | <img src=".\ResNet-LSTM-GCN\model1.png" alt="MGSTC" style="zoom: 50%;" /> |  |

 *Jinlei Zhang, Feng Chen, Zhiyong Cui, Yinan Guo, and Yadi Zhu*

------

<hr>
</details>



## [Demand Prediction](#content)
<details><summary> 2020 </summary>
[1] **Taxi Demand Prediction Using Parallel Multi-Task Learning Model.** TITS 2020. [note](), [paper](https://ieeexplore.ieee.org/document/9172100)

| Models  |  Modules   |                      Architecture                      | conclusion                                                   |
| :-----: | :--------: | :----------------------------------------------------: | :----------------------------------------------------------- |
| pmlLSTM | Multi-Task | ![pmlLSTm](./papers/2020/TITS/pmlLSTM/img/pmlLSTM.png) | This paper focus on the co-prediction of taxi pick-up and drop-off demands, and propose a parallel multi-task learning model, which can deal with shared features of multiple tasks simultaneously. In addition, this paper  design a novel taxi demand classifier to extract the time information hidden in the data, which embeds the time of a day feature into the forecasting model. |

*Chizhan Zhang, Fenghua Zhu, Xiao Wang, Leilei Sun, Haina Tang, Yisheng Lv*

---

<hr>
</details>


## [Travel time or Arrive time Prediction](#content)
<details><summary> 2020 </summary>

[1] **HetETA: Heterogeneous Information Network Embedding for Estimating Time of Arrival.** KDD 2020. [note](./papers/2020/KDD/HetETA/note.md), [paper](https://www.kdd.org/kdd2020/accepted-papers/view/heteta-heterogeneous-information-network-embedding-for-estimating-time-of-a), [github](https://github.com/didi/heteta)

| Models |    Modules     |                    Architecture                    | conclusion                                                   |
| :----: | :------------: | :------------------------------------------------: | :----------------------------------------------------------- |
| HetETA | GatedCNNs, GCN | ![HetETA](./papers/2020/KDD/HetETA/img/HetETA.png) | In this paper, traffic structure is constructed by digging deeper semantic information of traffic network. HetETA combines gated convolution neural networks and graph neural networks to capture the correlations in spatiotemporal information. |

*Huiting Hong, Yucheng Lin, Xiaoqing Yang, Zang Li, Kun Fu, Zheng Wang, Xiaohu Qie, Jieping Ye*

---

[2] **CompactETA: A Fast Inference System for Travel Time Prediction.** KDD 2020. [note](./papers/2020/KDD/CompactETA/note.md), [paper](https://www.kdd.org/kdd2020/accepted-papers/view/compacteta-a-fast-inference-system-for-travel-time-prediction)

|   Models   |                   Modules                    |                         Architecture                         | conclusion                                                   |
| :--------: | :------------------------------------------: | :----------------------------------------------------------: | :----------------------------------------------------------- |
| CompactETA | Graph attention network, Positional encoding | ![CompactETA](./papers/2020/KDD/CompactETA/img/CompactETA.png) | This paper use a compact model for real-time inference. The inference model use high level link representations as input feature, which is learnt on road network graph by a graph attention network equipped with positional encoding. These representations capture the spatiotemporal dependency between roads, and further encode the sequential information of the travel route. |

*Kun Fu, Fanlin Meng, Jieping Ye, Zheng Wang*

---
</details>



## [Speed Prediction](#content)

<details><summary> 2019 </summary>

[1] **[Graph WaveNet for Deep Spatial-Temporal Graph Modeling.](./papers/2019/IJCAI/GWN)** IJCAI 2019. [note](./papers/2019/IJCAI/GWN/note.md). [paper](https://arxiv.org/abs/1906.00121), [github](https://github.com/nnzhan/Graph-WaveNet)

| Models |              Modules               |                Architecture                 | conclusion                                                   |
| :----: | :--------------------------------: | :-----------------------------------------: | :----------------------------------------------------------- |
|  GWN   | GCN with adaptive Matrix,Gated TCN | ![GWN](./papers/2019/IJCAI/GWN/img/GWN.png) | This paper proposes a diffusion convolution formula with an adaptive adjacency matrix on the basis of DCRNN. During the training process, it also emphasizes that the structure of the graph changes dynamically. The paper uses two embedding vectors to dynamically learn the graph structure. Causal convolution is used to model time dependence. The overall structure of the model is similar to WaveNet. |

*Zonghan Wu, Shirui Pan, Guodong Long, Jing Jiang, Chengqi Zhang*

<hr>
</details>


# [Datasets](#content)

[1] GAIA Open Dataset: [link](https://outreach.didichuxing.com/research/opendata/)

[2] 智慧足迹: [link](http://www.smartsteps.com/)

## [Sensor data](#content)

[1] UK traffic flow datasets: [link](https://www.gov.uk/)

[2] Illinois traffic flow datasets: [link](http://www.travelmidwest.com/)

[3] PeMS: [link](http://pems.dot.ca.gov/), [Baidu Netdisk](https://pan.baidu.com/s/1c3NNV7nGnDylFJ9tBYUF0g) password:jutw | [PeMS Guide](https://github.com/Knowledge-Precipitation-Tribe/Urban-computing-papers/blob/master/PEMS.md)

## [Trajectory data](#content)

[1] Chengdu: [link](https://outreach.didichuxing.com/app-vue/TTItrajectory?id=1001)

[2] Xian: [link](https://outreach.didichuxing.com/app-vue/TTItrajectory?id=1001)

## [Others](#content)

[1] Weather and events data: [link](https://www.wunderground.com/)

[2] Weather and climate data: [link](https://www.ncdc.noaa.gov/data-access)

[3] NSW POI data: [link](https://sdi.nsw.gov.au/catalog/search/resource/details.page?uuid=%7BC41F6FE5-1C56-4556-%209EC6-EC9BD7094BBB%7D)

[4] Road network data: [link](http://networkrepository.com/road.php)

[5] NYC OpenData: [link](https://opendata.cityofnewyork.us/)

[6] METR-LA: [link](http://geohub.lacity.org/datasets/traffic-data?geometry=-119.170%2C33.900%2C-117.193%2C34.298), [Baidu Netdisk](https://pan.baidu.com/s/1g9yxZMDVf9nI0eN-ixeiPQ) password:xsz5

[7] TaxiBJ: [link](https://github.com/TolicWang/DeepST/tree/master/data/TaxiBJ), [Baidu Netdisk](https://pan.baidu.com/s/1aoi7gEkFQFn2MTYlGuc7Iw) password:sg4n

[8] BikeNYC: [link](https://www.citibikenyc.com/system-data), [Baidu Netdisk](https://pan.baidu.com/s/1SdSPWu5c761H3e8XjtzuaA) password:lmwj

[9] NYC-Taxi: [link](https://www1.nyc.gov/site/tlc/about/tlc-trip-record-data.page), [Baidu Netdisk](https://pan.baidu.com/s/1W2UV-xiDG_wbM9tuPvfrsA) password:022y

[10] NYC-Bike: [link](https://www.citibikenyc.com/system-data)

[11] San Francisco taxi: [link](https://crawdad.org/)

[12] Chicago bike: [link](https://www.divvybikes.com/system-data)

[13] BikeDC: [link](https://www.capitalbikeshare.com/system-data)

# [Experts](#content)

(排名不分先后)

[1] Yu Zheng: [link](http://urban-computing.com/yuzheng)

[2] Yanhua Li: [link](http://users.wpi.edu/~yli15/index.html)

[3] Xun Zhou: [link](https://www.biz.uiowa.edu/faculty/xzhou/)

[4] YaGuang Li: [link](http://www-scf.usc.edu/~yaguang/)

[5] Zhenhui Jessie Li: [link](https://faculty.ist.psu.edu/jessieli/Site/index.html)

[6] David S. Rosenblum: [link](https://www.comp.nus.edu.sg/~david/)

[7] Huaiyu Wan: [link](http://faculty.bjtu.edu.cn/8793/)

[8] Junbo Zhang: [link](https://zhangjunbo.org/)

[9] Shining Xiang:[link](https://scholar.google.com/citations?hl=zh-CN&user=0ggsACEAAAAJ)


# Contributors

