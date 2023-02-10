# Project structure

1. Data preparation
2. Initial CNN models
3. Data augmentation
4. Transfer learning?
5. Generating new cancer images
6. Performance?

# Guidlines: Computer Vision Lab (HSLU) 

## Project Format

The lab format is based on Enquiry Based Learning (EBL).

## What is "Enquiry Based Learning" (EBL)

EBL [1] describes an environment in which learning is driven by a process of enquiry owned by the student.
Starting with a ‘scenario’ and with the guidance of a facilitator, students identify their own issues and questions. They then examine the resources they need to research the topic, thereby acquiring the requisite knowledge. Knowledge so gained is more readily retained because it has been acquired by experience and in relation to a real problem.
It is essential that our students are educated for knowledge creation, lifelong learning and leadership. They will take on leading roles in their future working environments: directing change, asking important questions, solving problems and developing new knowledge.

## Characteristics of EBL

Learning is essentially student-centred, with an emphasis on group work and use of library, web and other information resources.
Lecturers become facilitators, providing encouragement and support to enable the students to take responsibility for what and how they learn.
Students reach a point where they are not simply investigating questions posed by others, but can formulate their own research topics and convert that research into useful knowledge.
Students gain not only a deeper understanding of the subject-matter, but also the knowledge-development and leadership skills required for tackling complex problems that occur in the real world.

## Benefits of EBL

Fundamentally, students are more engaged with the subject. Learning is perceived as being more relevant to their own needs, thus they are enthusiastic and ready to learn.
Students can expand on what they have learned by following their own research interests.
EBL allows students to develop a more flexible approach to their studies, giving them the freedom and the responsibility to organize their own pattern of work within the time constraints of the task.
Working within and communicating to a group are vital for a student’s employability.
Self-directed learning not only develops key skills for postgraduate study, but also leads to original thought that contributes to larger research projects, papers and publications.
For teaching staff, developing an EBL module helps to understand the learning process and the changing needs of students.

## Reading Material

The project is described in detail in chapter 8 of the book "Advanced Applied Deep Learning" by Umberto Michelucci. The PDF of the book can be found in the ILIAS page of the course. In particular, read chapter 8 as it gives a good overview of the data and hints on how to solve the problem.

## Goal of the Project

The goal of this project, and your task, is to build a machine learning pipeline to identify microscope images with cancer cells in it. You will do it by using techniques that you have learned in the course. The goal is not to get the best model or the highest accuracy, but to get experience in dealing with real data and all the challenges assocaited with the use case.

## Data

This data set represents a collection of textures in histological images of human colorectal cancer. It contains two files:
"Kather_texture_2016_image_tiles_5000.zip": a zipped folder containing 5000 histological images of 150 * 150 px each (74 * 74 µm). Each image belongs to exactly one of eight tissue categories (specified by the folder name).
"Kather_texture_2016_larger_images_10.zip": a zipped folder containing 10 larger histological images of 5000 x 5000 px each. These images contain more than one tissue type.

## Image format

All images are RGB, 0.495 µm per pixel, digitized with an Aperio ScanScope (Aperio/Leica biosystems), magnification 20x. Histological samples are fully anonymized images of formalin-fixed paraffin-embedded human colorectal adenocarcinomas (primary tumors) from our pathology archive (Institute of Pathology, University Medical Center Mannheim, Heidelberg University, Mannheim, Germany).

## Ethics statement

All experiments were approved by the institutional ethics board (medical ethics board II, University Medical Center Mannheim, Heidelberg University, Germany; approval 2015-868R-MA). The institutional ethics board waived the need for informed consent for this retrospective analysis of anonymized samples. All experiments were carried out in accordance with the approved guidelines and with the Declaration of Helsinki.


The dataset serves as a much more interesting MNIST or CIFAR10 problem for biologists by focusing on histology tiles from patients with colorectal cancer. In particular, the data has 8 different classes of tissue (but Cancer/Not Cancer can also be an interesting problem). 

The dataset is composed of two parts:
- The small images that will be used to test the classification models
- The big microscope images (5000x5000)

The first dataset is quite small but the second are much bigger (250 Mb and 700 Mb). You can get them on 
kaggle: https://www.kaggle.com/code/kmader/histology-mnist-csv-overview/data. The original data can be found on zenodo: https://zenodo.org/record/53169#.Y3R-ty8w3Lu
Instructions and Code


[1] http://www.ceebl.manchester.ac.uk/ebl/, Last Accessed 13th November 2022.
