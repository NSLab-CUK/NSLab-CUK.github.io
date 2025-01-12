---
layout: page
title: Syllabus of Graph Neural Networks (06838)
permalink: /lecture/syllabus/graph-neural-networks/eng
image: CUK_4Seasons.jpg
description: Welcome to the syllabus of the Graph Neural Networks (06838) class for the Department of Artificial Intelligence at the Catholic University of Korea.
---

<h5>Table of Contents</h5>
* TOC
{:toc}

***

## **1. Course Information**

- **Lecture Times:** Tuesday (Periods 2–3), Thursday (Period 3)  
- **Classroom:** Sophie Barat Hall B346

## **2. Instructor & TAs**

### **Instructor**
- **Name:** [O-Joun Lee](https://nslab-cuk.github.io/member/ojlee) (Professor)  
- **Office:** Michael Hall T404  
- **Email:** [ojlee@catholic.ac.kr](mailto:ojlee@catholic.ac.kr)  
- **Website:** [NSLab @ CUK](https://nslab-cuk.github.io/)  
- **Office Hour:** *TBA (by appointment or specific times)*

---

## **3. Course Description**

This course offers an in-depth exploration of **Graph Neural Networks (GNNs)**, a rapidly evolving area in machine learning and AI research. Students will learn the theoretical foundations of GNNs, examine state-of-the-art models, and apply them to real-world problems. Key topics include:

- **Foundations of Graph Theory** and their relevance to machine learning  
- **Graph Convolutional Networks (GCNs)**: architecture, training, and limitations (e.g., over-smoothing)  
- **Advanced GNN Models**: Graph Attention Networks (GATs), structure-preserving GNNs (e.g., GIN), Graph Transformers  
- **Graph Pooling Techniques**: DiffPool, SAGPool, hierarchical structure learning  
- **Graph Autoencoders & Generative Models**  
- **Dynamic & Heterogeneous GNNs**: handling evolving graph structures, relational GCNs, etc.  

By the end of this course, students will be able to:

1. Understand core concepts of graph theory as they apply to GNNs  
2. Develop, train, and evaluate various GNN models (GCNs, GATs, Transformers, etc.)  
3. Identify and address common GNN limitations  
4. Apply GNNs to tasks in NLP, social network analysis, bioinformatics, recommendation systems, and more  
5. Stay current with cutting-edge research trends in GNNs  

---

## **4. Course Materials**

- **Lecture Notes & Assignments:**  
  Materials are updated weekly on the course’s online learning platform (or the GitHub repository linked below).

- **Practice & Assignments Repository:**  
  <https://github.com/stars/NSLab-CUK/lists/graph-neural-networks>

---

## **5. Tentative Schedule**

| **Week** | **Topics**                                                           | **Key Concepts & Activities**                                                                                                  |
|:-------:|:---------------------------------------------------------------------|:------------------------------------------------------------------------------------------------------------------------------|
| **1**   | *Introduction to Graph Neural Networks*                              | - Motivation for GNNs <br/> - Node, Edge, and Graph Embeddings <br/> - Overview of Graph ML Landscape                         |
| **2**   | *Fundamentals of Graph Convolutional Networks (GCNs)*                | - Basic GCN Framework <br/> - Convolution Operation in GCNs <br/> - Propagation Rules                                        |
| **3**   | *Variants of GCNs and Limitations*                                   | - GraphSAGE <br/> - Over-smoothing, Over-squashing in GCNs                                                                   |
| **4**   | *Overcoming GCN Limitations*                                         | - Methods for handling over-smoothing <br/> - Scalability solutions                                                          |
| **5**   | *Introduction to Graph Attention Networks (GATs) I*                  | - GAT Basics <br/> - Attention Mechanisms in GATs                                                                            |
| **6**   | *Deep Dive into GATs II*                                             | - Multi-head Attention <br/> - Training GATs <br/> - Applications of GATs                                                    |
| **7**   | *Structure-Preserving GNNs I*                                        | - Motivation for Structure Preservation <br/> - Graph Isomorphism Networks (GIN)                                             |
| **8**   | **Mid-term Exam**                                                    | - Covers Weeks 1–7                                                                                                           |
| **9**   | *Structure-Preserving GNNs II*                                       | - Additional models and case studies                                                                                        |
| **10**  | *Introduction to Graph Transformers I*                               | - Transformers in NLP <br/> - “Attention Is All You Need” <br/> - Adapting Transformers for Graph Data                       |
| **11**  | *Introduction to Graph Transformers II*                              | - Graph Transformer Networks (GTN) <br/> - Applications of Graph Transformers <br/> - Case Studies                           |
| **12**  | *Graph Pooling Techniques*                                           | - DiffPool <br/> - SAGPool <br/> - Global Attention Pool <br/> - Hierarchical Graph Pooling                                  |
| **13**  | *Graph Autoencoders (GAEs) and Variational GAEs (VGAEs)*             | - Basic Framework of GAEs <br/> - Understanding VGAEs <br/> - Applications in Generation/Anomaly Detection                  |
| **14**  | *Handling Dynamic & Heterogeneous GNNs*                              | - Dynamic GCNs, Recurrent GNNs, EvolveGCN <br/> - Heterogeneous GCN (HGCN), Relational GCN (RGCN), HAN                        |
| **15**  | (Open/Review Week)*                                                 | - (Optional: Project presentations, guest lectures, or review)                                                               |
| **16**  | **Final Exam**                                                       | - Comprehensive coverage of Weeks 1–14                                                                                       |

*\* Week 15 may be reserved for additional reviews, project presentations, or special lectures at the instructor’s discretion.*  

---

## **6. Practices & Assignments**

- **Assignments:** Practice materials and problem sets will be posted on the [GitHub repository](https://github.com/stars/NSLab-CUK/lists/graph-neural-networks). Please submit all solutions via the course’s online platform by the stated deadlines.

### **Late Submission Policy**
- Assignments submitted **after** the deadline are capped at a grade of **B (8 points)**.  
- Failure to submit or excessively late submissions may result in **F (0 points)** for that assignment.

---

## **7. Evaluation**

| **Component**     | **Percentage** |
|:-----------------:|:--------------:|
| **Attendance**    | 10%           |
| **Assignments**   | 30%           |
| **Mid-term Exam** | 30%           |
| **Final Exam**    | 30%           |

### **Grading Scale**
- **A**: 80–100  
- **B**: 60–80  
- **C**: < 60  
- **F**: Absence from exams  

*(Exact cutoffs may be slightly adjusted at the instructor’s discretion.)*

---

## **8. Academic Integrity & Plagiarism**

- **Policy:** Plagiarism or any form of academic dishonesty (e.g., copying code or solutions without proper citation) will not be tolerated.
- **Consequences:** Violations may result in penalties up to and including failing the assignment/exam or the entire course.
- **Guidelines:**  
  1. Complete your own work.  
  2. Properly cite any external sources.  
  3. If you have questions on citation or collaboration policies, consult the instructor or TAs in advance.

---

## **9. Exams**

- **Mid-term Exam (Week 8):** Details (format, scope) will be announced.  
- **Final Exam (Week 16):** Comprehensive assessment covering key topics.  
- **Make-Up Policy:** Only students with valid, documented reasons (e.g., illness) may request make-up exams.

---

## **10. Contact & Office Hours**

- **Instructor Office Hour:** *TBA.* Students are encouraged to email for appointments or questions.  
- **TA Office Hour:** *TBA.* The TAs are available to help with assignments, projects, or any course-related queries.

---

**Note:** This syllabus is subject to minor revisions. Any changes will be announced through the online platform or email. Students are responsible for staying up to date. We look forward to an engaging semester exploring the world of Graph Neural Networks!
