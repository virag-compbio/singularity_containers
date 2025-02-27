## Singularity Containers
This repo contains singularity definition files for routine bioinformatics analyses

Basically, this repo hosts Singularity definition (.def) files for a variety of bioinformatics applications. These definition files allow you to build portable and reproducible Singularity containers, enabling seamless deployment of bioinformatics tools across different environments.

### Why Singularity?
Singularity is a powerful containerization platform widely used in high-performance computing (HPC) and bioinformatics. It allows you to package software, dependencies, and workflows into a single container, ensuring consistency and reproducibility across systems. Unlike other containerization tools, Singularity is designed with security and ease of use in mind, making it ideal for shared and multi-user environments.

### What is contained in this repo?
This repository contains .def files for building Singularity images (.sif) for a range of bioinformatics tools. Each .def file defines the base image, software dependencies, and installation steps required to create a functional container. While the actual .sif images are not included due to size constraints, these can be easily built using the .def files

### How to use
1. Install Singularity - ensure that singularity is installed on your system. For installation instructions, you may need to refer to the official documentation for singularity
2. Build containers - use the .def files in this repository to build singularity images. Here is an example:
```
sudo singularity build my_image.sif my_image_definition.def
```
3. Run containers: Once the containers have been built, they can be used with the following command:
```
singularity run my_image.sif
```

#### Contributions
Contributions to this repository are very welcome!
If you have a .def file for a bioinformatics tool that isn't already included, feel free to submit a pull request. Please ensure your definition file is well-documented and follows best practices for Singularity containerization.
