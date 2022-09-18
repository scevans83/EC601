# The Use of Artificial Intelligence for Detecting and Localizing Fractures in the Cervical Spine
## Sophia Evans




### Problem Statement/Applications

Machine learning techniques can be used to create and refine models for not just detecting but localizing fractures in the cervical spine. Effectively utilizing this process will increase both efficiency and accuracy in providing care to patients with suspected cervical spine fractures. 

Over 1.5 million spinal fractures occur every year in the United States. Of these, around 25000 are located in the uppermost seven vertebrae, known as the cervical spine (Lasfargues, 1995). Although all spinal fractures are dangerous due to their proximity to the spinal cord, cervical fractures are especially likely to cause death, as injuries to the spinal cord in the neck can cause paralysis in areas like the lungs [1].

Cervical spine fractures are typically diagnosed with computed tomography (CT) scans. CT scans produce images of cross sections of the body by taking many x-ray measurements from different angles [2]. For fractures, the ability to view multiple planes of a suspect area is beneficial around joints, such as in the neck, or in locations that may also be affected by other problems, such as osteoporosis [2]. 

However, CT scans do not always provide a clear view of fractures. Some populations, such as the elderly, are more prone to bone disorders or degeneration that may obscure any present fractures [3]. This is problematic because it increases the likelihood of false negative results and, therefore, the risk of paralysis or death due to not receiving treatment. The elderly population is increasingly experiencing cervical spine fractures, so it is vital to ensure that there is a way of mitigating these potentialities [4]. By using machine learning techniques to create and refine models for not just detecting but localizing fractures, patients will be able to receive more accurate care in a shorter amount of time. 


### Current Research

Past research has shown that neural networks can detect subtle patterns that humans cannot differentiate [7,8]. For example, a 2018 study showed that artificial intelligence could successfully identify cellular structures in images in which contrast was too low for human eyes to distinguish the slight differences [7]. 

Current research primarily focuses on the use of convolutional neural networks (CNN), which use layers of artificial “neurons” to process information from images and classify them based on whatever characteristics the CNN determines to be important. Unlike a typical feed-forward neural network, CNNs use multiple Convolution Layers to extract information about edges, color, and other features within the image [5]. 

Although artificial intelligence has been used in fracture detection for several years, the first study about the use of CNNs in cervical spine fracture detection was not published until 2021 [5]. The researchers evaluated the sensitivity of a CNN called C-spine against that of trained radiologists. The CNN was trained on around 12,000 CT scans of the cervical spine, 80% negative and 20% positive for fractures. For testing, just under 700 scans with a similar negative/positive rate were given to both the CNN and a group of radiologists. The CNN produced similar results to those of the cohort of radiologists, around 92% and 95% accuracy respectively. Interestingly, although the CNN was more likely to produce a false-negative result, the CNN and the radiologists showed similar patterns in location of false-negatives (Fig 1). 
 

 
 
![Images showing the location of false-negative and -positive results for radiologists and the CNN [5]. Each red dot represents a false result.](https://user-images.githubusercontent.com/60391096/190924194-838c897d-7f0c-4890-9bf2-c17141c5751b.png)

 
> **Fig 1** Images showing the location of false-negative and -positive results for radiologists and the CNN. Each red dot represents a false result. (citation needed)




However, in a typical clinical research setting, the incidence of fracture-positive scans would generally be much lower, and upon extrapolating the sample size and results to a dataset with a lower fracture incidence, accuracy rates decreased significantly for both radiologists and CNN [5]. In any case, further research will be needed to refine the CNN. 

Despite this limitation, the study showed promise for using artificial intelligence to detect cervical fractures. The CNN was able to process each scan and produce results in approximately one-fifth of the time that a radiologist needed to perform the same task [5]. In addition, as seen in Figure 1, the study showed likely locations of false results from the CNN, allowing doctors to examine those areas more critically while ruling out unlikely fracture locations [5]. Thus, even with the lower accuracy rates of the demonstrated model, the CNN would still be able to save time in clinical settings. 

### Current Open-Source Solutions

This topic is also a growing source of interest in open-source communities. Another facet that is being explored is the issue of localizing fractures or determining in which of the seven cervical vertebrae a fracture is located. Radiologists, neurologists, neurosurgeons, and other medical professionals use their knowledge of cervical anatomy to reliably determine which vertebra a given “slice” is depicting. However, depending on the specialty of the medical professional in question, they may not be as accurate in estimating the location within the cervical spine. In this case, they would generally rely on labels placed by a radiologist, which increases the time before a patient can receive stabilizing care. Use of artificial intelligence to provide locating information on CT scans would help to minimize this effect. 

On the Kaggle contest page “RSNA 2022 Cervical Spine Fracture Detection”, Vladimir Slaykovskiy posted a toolset to identify the location or a given CT image within the cervical spine, with a claim of 95% accuracy [9]. Their program uses EfficientNet-V2 convolutional neural networks as a basis for the multi-label classification models and produces vertebrae predictions.

### Conclusion

In conclusion, the use of machine learning and artificial intelligence to detect cervical spine fractures is a very promising field of research. In future research, it would be interesting to explore the ability to use machine learning to differentiate specific types of fracture, and whether it is likely to have corresponding ligamentous injury. In addition, some cervical spine fractures are considered more stable than others, so it would be useful to see if a neural network can be used to determine the potential stability of an injury.

### References

[1] J. Lasfargues, D. Custis, F. Morrone, J. Carswell and T. Nguyen, "A model for estimating spinal cord injury prevalence in the United States", Spinal Cord, vol. 33, no. 2, pp. 62-68, 1995. Available: 10.1038/sc.1995.16 [Accessed 18 September 2022].

[2] "Computed Tomography (CT)", Nibib.nih.gov, 2022. [Online]. Available: https://www.nibib.nih.gov/science-education/science-topics/computed-tomography-ct. [Accessed: 18- Sep- 2022].

[3] C. Yeo, I. Jeon and S. Kim, "Delayed or Missed Diagnosis of Cervical Instability after Traumatic Injury: Usefulness of Dynamic Flexion and Extension Radiographs", Korean Journal of Spine, vol. 12, no. 3, p. 146, 2015. Available: 10.14245/kjs.2015.12.3.146 [Accessed 18 September 2022].

[4] M. Yamashita et al., "Mortality and complications in elderly patients with cervical spine injuries", Injury, vol. 53, no. 6, pp. 2114-2120, 2022. Available: 10.1016/j.injury.2022.04.015 [Accessed 18 September 2022].

[5] S. Saha, “A comprehensive guide to Convolutional Neural Networks - the eli5 way,” Medium, 17-Dec-2018. [Online]. Available: https://towardsdatascience.com/a-comprehensive-guide-to-convolutional-neural-networks-the-eli5-way-3bd2b1164a53. [Accessed: 18-Sep-2022]. 

[6] J. Small, P. Osler, A. Paul and M. Kunst, "CT Cervical Spine Fracture Detection Using a Convolutional Neural Network", American Journal of Neuroradiology, vol. 42, no. 7, pp. 1341-1347, 2021. Available: 10.3174/ajnr.a7094 [Accessed 18 September 2022].

[7] C. Ounkomol, S. Seshamani, M. M. Maleckar, F. Collman, and G. R. Johnson, “Label-free prediction of three-dimensional fluorescence images from transmitted-light microscopy,” Nature Methods, vol. 15, no. 11, pp. 917–920, 2018. 

[8] Y. Wang and M. Kosinski, "Deep neural networks are more accurate than humans at detecting sexual orientation from facial images.", Journal of Personality and Social Psychology, vol. 114, no. 2, pp. 246-257, 2018. Available: 10.1037/pspa0000098 [Accessed 18 September 2022].

[9] V. Slaykovskiy, "PyTorch-EffNetV2 vertebrae detection (acc: 0.95)", RSNA 2022 Cervical Spine Fracture Detection | Kaggle, 2022. Available: https://www.kaggle.com/embed/vslaykovsky/pytorch-effnetv2-vertebrae-detection-acc-0-95
