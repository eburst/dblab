---
title: "Database & Data Mining Lab - Research"
layout: textlay
excerpt: "Database & Data Mining Lab - Research"
sitemap: false
permalink: /research/
---

# Research

**Conversational, Self-tuning DBMS** In order for a general user to use a database management system (DBMS), the user needs to be proficient in handling schema, which is the structure of a database, and SQL, which is a query language. However, the general public does not know SQL and it is not easy even for a computer major to write an SQL query that accurately reflects their intentions. In addition, it is difficult for users of existing DBMSs to check whether they have properly written SQL queries. Even if the user writes the SQL query correctly, if there is no result returned by the DBMS, the user may not be sure that he or she wrote the SQL query correctly.

On the other hand, DBMS tuning is an important task that greatly affects query processing performance. Since it requires advanced knowledge of DBMS, expert database administrators (DBAs) are mainly responsible for the task. However, since the DBA’s salary is high, it is practically difficult to hire a DBA in a small company. Moreover, as the DBMS structure becomes more complex, tuning becomes difficult and tedious even for the DBAs.

The intelligent DBMS proposed to be developed in this project effectively solves the two problems mentioned above. The intelligent DBMS provides a natural language interface that can be easily accessed by users who do not have deep knowledge of DBMS and do not know SQL. In addition, non-experts can easily tune the DBMS, so individuals or small and medium-sized enterprises (SMEs) who are burdened with DBA employment can use it at a lower cost.

<iframe width="480" height="270" src="https://www.youtube.com/embed/CbpzMidK9Ms" frameborder="0" allowfullscreen></iframe>
<iframe width="480" height="270" src="https://drive.google.com/file/d/1qR64-Nhyth0GSFwbTFtHS9ChV89Rd_wS/preview" frameborder="0" allowfullscreen></iframe>

<br>
**Ultrafast Graph DBMS enhanced by Deep Learning** This study aims to develop an in-memory graph DBMS with major system components optimized by deep learning. Unlike the existing heuristic-based works, we use deep learning techniques for engine components. First, by synthesizing various intermediate result prediction models, it supports queries with a large number of joins and query plan optimizations including multi-graph query optimization. Second, it provides graph partitioning that minimizes workload processing cost based on deep learning modeling of query processing cost for the partitioned graph. Third, it optimizes graph transaction processing in real-time using lightweight deep learning techniques. Finally, for the system usability, it provides a query interface that automatically generates a regular path query by receiving examples of the result for a regular path query from a user. In other words, this system uses deep learning techniques to simultaneously improve both usability and performance optimization.

<iframe width="480" height="270" src="https://www.youtube.com/embed/OHOFLjmuinw" frameborder="0" allowfullscreen></iframe>

<br>
**Next-generation Distributed Graph DBMS** A distributed graph DBMS for intelligent processing of big graphs is a system that can raise the competitiveness of big data and artificial intelligence-based business. The system can process important graph applications by supporting efficient storage, analysis, and machine learning of large graphs on cloud-based distributed machines.

The three key queries for graph applications are graph pattern mining, graph analytics, and graph learning. However, the existing graph DBMSs have the following problems in supporting key queries: 1) Query processing is inefficient because native graph storage is not used. 2) Scalability is limited due to in-memory-based processing. 3) There is no integrated graph application processing involving the above three key queries.

Our goal is to develop a next-generation graph DBMS that can support graph applications mixed with three key graph queries on one system and provides scalable and efficient high-speed query processing for big graphs. The main components of the system are 1) Big/Dynamic native property graph storage, 2) Distributed and disk-based scalable, an efficient graph query engine, 3) Distributed graph neural network training and inference engine, 4) Integrated API library, and 5) Interactive query service.
<iframe width="480" height="270" src="https://www.youtube.com/embed/dIZshMyq7TE" frameborder="0" allowfullscreen></iframe>

<br>
**Automatic Realistic Image Generation (CVPR2022, Neurips2022)** For autoregressive (AR) modeling of high-resolution images, vector quantization (VQ) represents an image as a sequence of discrete codes. A short sequence length is important for an AR model to reduce its computational costs to consider long-range interactions of codes. However, we postulate that previous VQ cannot shorten the code sequence and generate high-fidelity images together in terms of the rate-distortion trade-off. In this study, we propose the two-stage framework, which consists of Residual-Quantized VAE (RQ-VAE) and RQ-Transformer, to effectively generate high-resolution images. Given a fixed codebook size, RQ-VAE can precisely approximate a feature map of an image and represent the image as a stacked map of discrete codes. Then, RQ-Transformer learns to predict the quantized feature vector at the next position by predicting the next stack of codes. Thanks to the precise approximation of RQ-VAE, we can represent a 256×256 image as 8×8 resolution of the feature map, and RQ-Transformer can efficiently reduce the computational costs. Consequently, our framework outperforms the existing AR models on various benchmarks of unconditional and conditional image generation. Our approach also has a significantly faster sampling speed than previous AR models to generate high-quality images.

<a href="https://openaccess.thecvf.com/content/CVPR2022/papers/Lee_Autoregressive_Image_Generation_Using_Residual_Quantization_CVPR_2022_paper.pdf"><b>cvpr paper</b></a> <br>
<a href="https://github.com/kakaobrain/rq-vae-transformer"><b>code link</b></a>


### ... and more.
