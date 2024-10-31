---
title: "Yang's AiLearn Lab - Vacancies"
layout: textlay
excerpt: "Openings"
sitemap: false
permalink: /vacancies
---


#  Open Position: Undergraduate Summer Research Student
## Undergraduate Summer Research Project: Training Large Language Models from Scratch 

### 1. Introduction to Large Language Models (LLMs)  
Large Language Models (LLMs) are advanced AI systems designed to understand and generate human-like text. They power applications like chatbots, language translation, summarization, and even creative writing. This project provides students with hands-on experience in training an LLM, focusing on foundational concepts, tools, and the computational resources needed to bring these models to life. If you are interested, please send me email along with your resume and transcript.

### 2. Project Goals  
This project aims to:

- Provide students with practical knowledge in LLM training, from data preprocessing to resource management.
- Teach students to use Compute Canada’s high-performance computing resources, including A100 and H100 GPUs.
- Engage students in exploring methods for training LLM from scratch, handling large datasets, and managing training complexity.

### 3. Overview of Training Requirements

**1. Compute Resources**  
We will use Compute Canada’s high-performance GPUs (A100 and H100) to handle the computational intensity of training large models. These GPUs are ideal for LLM training as they offer:

- High memory bandwidth to process large batches and sequences.
- Support for FP16 (half-precision) and BF16 operations, essential for training efficiency.

**2. Model Training Framework**  

We’ll be using **Megatron-LM**, a framework developed by NVIDIA specifically for training large models across multiple GPUs. Megatron-LM supports distributed data parallelism and model parallelism, crucial for managing the massive model sizes in LLMs.

**3. Storage and Data Pipeline**  

- **Dataset**: Large language datasets like The Pile or Common Crawl will provide the text corpus required to train the model.
- **Data Preprocessing Tools**: We’ll use tokenization techniques like Byte Pair Encoding (BPE) and SentencePiece to convert raw text into manageable tokens.
- **High-Speed Storage**: SSDs or NVMe are necessary to ensure data is read and written quickly, preventing bottlenecks during training.

### 4. Training Setup

#### 4.1 Distributed Training
Training an LLM requires multiple GPUs working in tandem:

- **Model Parallelism** splits the model across GPUs, allowing each GPU to handle different layers or sections of the model.
- **Data Parallelism** divides the data among GPUs, so each GPU processes a unique batch simultaneously.

#### 4.2 Mixed-Precision Training  
To efficiently utilize the computational power of the A100 and H100 GPUs, we use mixed-precision (FP16/BF16) training. This technique allows faster computations and reduces memory usage without compromising accuracy.

#### 4.3 Job Scheduling with SLURM  
To manage resources effectively on Compute Canada’s clusters, we use SLURM for scheduling. This allows us to allocate GPUs, manage distributed jobs, and track resource usage.

### 5. Monitoring and Logging

To track the progress of training and monitor resource utilization:

- **TensorBoard or Weights & Biases** for visualizing training metrics, including loss, accuracy, and GPU usage.
- **NVIDIA-smi and Prometheus** for GPU-specific monitoring.

### 6. Hyperparameter Tuning

Hyperparameter tuning is an essential part of optimizing LLM performance. Key hyperparameters include:

- **Learning Rate**: Determines the step size for each update in training.
- **Batch Size**: Affects how much data the model processes at once.
- **Model Size**: Refers to the number of layers and attention heads in the model, impacting both performance and computation cost.

### 7. Checkpointing and Model Management

Checkpointing helps save the model's progress periodically, ensuring that in case of interruptions, training can resume from a recent checkpoint:

- **Frequency of Checkpoints**: Ideally, every few hours or after a set number of steps.
- **Validation Checks**: To assess the model’s learning, we periodically evaluate it on a small validation set.

### 8. Fine-Tuning and Evaluation

Once the model is pre-trained, fine-tuning on a task-specific dataset allows it to specialize in certain tasks. For instance:

- **Text Classification**: Fine-tune on a labeled dataset to classify sentiments.
- **Summarization**: Fine-tune to produce concise summaries from long texts.

### 9. Learning Outcomes for Participants  
By the end of this project, students will:

- Understand the computational and data requirements for LLM training.
- Gain hands-on experience with distributed training and model parallelism using GPUs.
- Develop skills in managing and optimizing resources for high-performance training.

### 10. Research Opportunities  
Beyond learning practical skills, this project offers insights into advanced areas of AI research, with applications across healthcare, finance, media, and more. Students can explore pathways for internships, graduate research, and industry projects related to large-scale language models and their applications. 


<!---
# Open positions

**We are currently open for PhD and postdoc applications related to our ERC CoG grant. The positions are mostly related to the Electron Pair Microscopy projects.**

We are  looking for new group members with passion, talent, and grit!

You will have the chance to work on the grand challenges of condensed matter physics, often at the interface of instrumental design and new physics. You will be involved in determining the important and interesting questions, creating and improving instrumental setups, performing measurements, and making discoveries.

### Past open positions

You find the past job openings here:
[Opening 1]({{ site.baseurl }}/downloads/GeneralPostdoc_2019_v01.pdf),
[Opening 2]({{ site.baseurl }}/downloads/PPMS_PhD_2019_v01.pdf),
[Opening 3]({{ site.baseurl }}/downloads/PD.pdf),
[Opening 4]({{ site.baseurl }}/downloads/PHD1.pdf),
[Opening 5]({{ site.baseurl }}/downloads/PHD2.pdf).

### Applications for PhD and Postdoc positions
If you are interested in working with us as a PhD student or postdoc, please send me an [email](mailto:milan.allan@gmail.com). State briefly why you are interested and attach a CV, including information about the grades you had as an undergraduate. No need for a separate cover letter or certificates. **Important**: please insert _"Application PhD"_ or _"Application Postdoc"_ in the subject line. If you are applying to a specific advertisement, note this in your email.

We especially welcome postdocs with fellowships. I'd be happy to support you, also after you apply to our group. Take a look at the [veni fellowship](https://www.nwo.nl/en/calls/nwo-talent-programme-veni-science-domain) or the Marie Curie fellowship (currently closed, next deadline probably Fall 2021, [here is last years call]({{ site.baseurl }}/downloads/h2020-wp1820-msca_en.pdf)). In many country, there are also fellowships available for outdoing postdocs.**


### Master projects for Leiden University students
If you are a Master student at Leiden University looking for a Master project, contact me (or any group member) per email or stop by my office.

### Bsc / Master students from elsewhere
If you are interested in pursuing a Master degree at Leiden University, see [mastersinleiden.nl](http://www.mastersinleiden.nl/programmes/physics/en/introduction). Sometimes, we take master students or summer interns if we get exceptional applicants (this usually means very good grades and a personal recommendation).


<figure>
<img src="{{ site.url }}{{ site.baseurl }}/images/picpic/Gallery/DSC_0696.jpg" width="95%">
</figure>
-->
