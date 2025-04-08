# visual-categorisation-analysis
this repository contains supplementary materials for a cognitive neuroscience lab report examining category-selective brain activity in response to visual face and object stimuli using functional magnetic resonance imaging (fMRI). The study employed an event-related localiser design and general linear model (GLM) analysis implemented in SPM12.
the goal was to identify distinct cortical regions involved in face and object perception and explore potential lateralisation effects within the ventral visual stream.

contents
tables
`2nd_level_face.xlsx` – cluster table for the face condition
`2nd_level_object.xlsx` – cluster table for the object condition
`face - object.xlsx` – contrast results for Face > Object
`object - face.xlsx` – contrast results for Object > Face
each Excel file includes peak MNI coordinates, cluster sizes, and anatomical labels, derived from SPM results and neuroanatomical atlases.
contrasts
con_0001.nii`- face condition contrast
`con_0002.nii` – object condition contrast  
`con_0003.nii` – face > object contrast  
`con_0004.nii` – object > face contrast  
these contrast images were used for group-level activation maps and figure generation in the manuscript.

analysis
preprocessing and statistical analysis were performed using SPM12 in MATLAB (R2024a). the steps included:
Realignment
Coregistration to T1-weighted structural image
Segmentation and normalization to MNI space
Smoothing with 8mm FWHM Gaussian kernel
First-level GLM using canonical HRF
Second-level group analysis using one-sample t-tests
contrasts were thresholded at p < 0.01 (uncorrected) with a cluster extent threshold of 50 voxels.

notes
the design was a slow event-related paradigm (12s stimuli, interleaved with 12s grey screen).
no ROI analysis was performed, although attempted, but full cluster-level data is included.
all data anonymised and stripped of identifying information.
