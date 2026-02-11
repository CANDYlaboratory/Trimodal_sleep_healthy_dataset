# Trimodal_sleep_healthy_dataset

This dataset is a subset of the subjects reported in the "Simultaneous EEG-PET-MRI identifies temporally coupled and spatially structured brain dynamics across wakefulness and NREM sleep" paper.

Under each subject folder: 

"/func" contains the parcellated cortical fMRI data in Schaefer's 200 and 300 parcellations, seperated by hemispheres. "Saseg.mat" containes the parcellated subcortical fMRI data in freesurfer's subcortical segmentation. The shared fMRI data went through a standard preprocessing pipeline with motion correction, slice timing correction, and distortion correction. 

"/pet" contains the parcellated cortical FDG-PET data in Schaefer's 200 and 300 parcellations, seperated by hemispheres. "Saseg.mat" containes the parcellated subcortical FDG-PET data in freesurfer's subcortical segmentation. The shared FDG-PET data were motion-corrected. 

"PET_fMRI_onset_time_difference.mat" denotes the time difference between PET signal and fMRI signal onset in seconds. PET acquisitions always started before fMRI acquisitions.

"sleepscore_fMRIonset.mat" marks the sleep/arousal stage of the subject identified through EEG signals. The sleep scores are matched with fMRI signal onset time. 0 = wake, 1 = NREM stage 1, 2 = NREM stage 2, 3 = NREM stage 3, -1 = artifact.

Please see "s200+s300_parcellations_list.mat" for the order of ROIs in each parcellated cortical fMRI/PET data. E.g., "s200_7net_lh_list" contains information of the ROI order of "S_s200_7net_lh.mat" files. 

Please see "FreeSurferColorLUT.txt" for the order of ROIs in "Saseg.mat" files. 
