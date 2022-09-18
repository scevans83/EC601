# The Use of Artificial Intelligence for Detecting and Localizing Fractures in the Cervical Spine
## Sophia Evans




### Problem Statement/Applications

Machine learning techniques can be used to create and refine models for not just detecting but localizing fractures in the cervical spine. Effectively utilizing this process will increase both efficiency and accuracy in providing care to patients with suspected cervical spine fractures. 

Over 1.5 million spinal fractures occur every year in the United States. Of these, around 25000 are located in the uppermost seven vertebrae, known as the cervical spine (Lasfargues, 1995). Although all spinal fractures are dangerous due to their proximity to the spinal cord, cervical fractures are especially likely to cause death, as injuries to the spinal cord in the neck can cause paralysis in areas like the lungs. (expand on this).

Cervical spine fractures are typically diagnosed with computed tomography (CT) scans. CT scans produce images of cross sections of the body by taking many x-ray measurements from different angles. For fractures, the ability to view multiple planes of a suspect area is beneficial around joints, such as in the neck, or in locations that may also be affected by other problems, such as osteoporosis. 

However, CT scans do not always provide a clear view of fractures. Some populations, such as the elderly, are more prone to bone disorders or degeneration that may obscure any present fractures. This is problematic because it increases the likelihood of false negative results and, therefore, the risk of paralysis or death due to not receiving treatment. The elderly population is increasingly experiencing cervical spine fractures (source), so it is vital to ensure that there is a way of mitigating these potentialities. By using machine learning techniques to create and refine models for not just detecting but localizing fractures, patients will be able to receive more accurate care in a shorter amount of time. 

### Current Research

Past research has shown that neural networks can detect subtle patterns that humans cannot differentiate. For example, a 2018 study showed that artificial intelligence could successfully identify cellular structures in images in which contrast was too low for human eyes to distinguish the slight differences (Ounkomol et al. 2018). 

Current research primarily focuses on the use of convolutional neural networks (CNN), which use layers of artificial “neurons” to process information from images and classify them based on whatever characteristics the CNN determines to be important. Unlike a typical feed-forward neural network, CNNs use multiple Convolution Layers to extract information about edges, color, and other features within the image (). 

Although artificial intelligence has been used in fracture detection for several years (), the first study about the use of CNNs in cervical spine fracture detection was not published until 2021. The researchers evaluated the sensitivity of a CNN called C-spine against that of trained radiologists. The CNN was trained on around 12,000 CT scans of the cervical spine, 80% negative and 20% positive for fractures. For testing, just under 700 scans with a similar negative/positive rate were given to both the CNN and a group of radiologists. The CNN resulted in a sensitivity of 79%, while the radiologists’ sensitivity was higher, at 93%. Interestingly, although the CNN was more likely to produce a false-negative result, the CNN and radiologists showed similar patterns in location of false-negatives (fig 1). 

 
 
![Images showing the location of false-negative and -positive results for radiologists and the CNN. Each red dot represents a false result.](https://user-images.githubusercontent.com/60391096/190924194-838c897d-7f0c-4890-9bf2-c17141c5751b.png)

 
> **Fig 1** Images showing the location of false-negative and -positive results for radiologists and the CNN. Each red dot represents a false result. (citation needed)




However, in a typical clinical research setting, the incidence of fracture-positive scans would generally be much lower. Upon extrapolating the sample size and results to a dataset with a lower fracture incidence, the sensitivity rate dropped significantly for both the radiologists and the CNN. In any case, further research will be needed to refine the CNN. 

Despite this limitation, the study show>ed promise for using artificial intelligence to detect cervical fractures. The CNN was able to process each scan and produce results in approximately one-fifth of the time that a radiologist needed to perform the same task. In addition, as seen in Figure 1, the study showed likely locations of false results from the CNN, allowing doctors to examine those areas more critically while ruling out unlikely fracture locations. Thus, even with the lower sensitivity rates of the demonstrated model, the CNN would still be able to save time in clinical settings. 

### Current Open-Source Solutions

This topic is also a growing source of interest in open-source communities. Another facet that is being explored is the issue of localizing fractures or determining in which of the seven cervical vertebrae a fracture is located. Radiologists, neurologists, neurosurgeons, and other medical professionals use their knowledge of cervical anatomy to reliably determine which vertebra a given “slice” is depicting. However, depending on the specialty of the medical professional in question, they may not be as accurate in estimating the location within the cervical spine. In this case, they would generally rely on labels placed by a radiologist, which increases the time before a patient can receive stabilizing care. Use of artificial intelligence to provide locating information on CT scans would help to minimize this effect. 

### Conclusion

Potential paths: determine what kind of fracture- hangman, car(?), sublux, compression, etc?? Considered a stable fracture or not? (fracturing bones in the spine that don’t mean head will fall off- e.g. could have tiny little teardrop fracture that implies a major injury to spine bc ligaments are damages) (stability is able to function with no pain) (try to infer accompanying ligamentous injury from type of fracture) (ligamentous injury means head could turn too far and sever spinal cord, lots of fun stuff)


*fix sensitivity vs accuracy
