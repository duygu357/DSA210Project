# DSA210Project
# 
## Overview
In recent years, materials science has gained significant attention due to rapidly evolving technological developments. One key driver of this progress is the use of computational methods to guide scientists toward interesting material properties to explore. Instead of conducting 100 different experiments, researchers can now rely on machine learning (ML) models to highlight 10 promising materials for targeted testing. This approach greatly enhances efficiency and accelerates discovery.

## Project Motivation
Through this project, I aim to make a small contribution in the field of mechanical properties—specifically the elastic modulus of metals. Mechanical properties are critical in designing durable structures, and metals are often the first choice when we think of strength and resilience. The elastic modulus, in particular, is a core parameter for numerous strength calculations, so focusing on this property makes practical sense for both theoretical and real-world applications.

### "Modeling an Elastic Modulus Estimation Model"
This project consists of four main phases:

## 1.Data Collection
- Collect the necessary features of metallic materials from open property databases, parsing and organizing the data using Python.
- Most of the data will be taken from >> "https://next-gen.materialsproject.org/" << which is a open-source with massive dataset.
- Crystallographic Information File (CIF) and elastic modulus of the materials will be dowloaded and parse with "CifParser" in "Pymatgen" library. With CIF files it's possible to reach various features through Magpie data library in Python.
- In conclusion, Necessary informations will be extracted through MaterialsProject database to parse through existing Python libraries.

## 2.Data Cleaning and Analysis
- Visualize the collected data to detect any anomalies or inconsistencies. Materials showing unusual patterns will be examined against typical expectations, ensuring the dataset is both reliable and representative.

## 3.Training and Optimization
- Train machine learning models to estimate the elastic modulus of metals. This phase also involves fine-tuning model parameters to achieve optimal performance.

## 4.Error Metrics and Finalizing the Model
- Compare various error metrics and benchmark the results against similar studies. The goal is to select the best-performing model and finalize its configuration for future use.

By following these steps, it's aimed to develop a robust, data-driven model capable of accurately estimating the elastic modulus for different metals.
