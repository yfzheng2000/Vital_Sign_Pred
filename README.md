# Vital_Sign_Pred
Paper: Hybrid Neural Network Models to Estimate Vital Signs from Facial Videos

Instruction to infer vital signs with the pre-trained models:
(1) download the test data file: 'Norm_30Frm_ValIdx250.npz'-- One sample (idx=250) from the test subset: X normalized to [-1,1], Y ground truth (not scaled). Note: Users are Not permitted to distribute or publish this data.
(2) download the pre-trained weights of 'Mdl_a': 'Mdl_a.weights.h5', 6.2GB -- cannot uploaded here due to its size. The downloading link for zipped weights file: 
(3) 'hybrid_face_vital.ipynb': run this code in Jupyter Lab or Notebook to Predict Vital Signs from Facial Videos.

PC/GPU configuration for our experiments: 
All models were implemented using Python 3.9 and TensorFlow 2.19 (Keras 3), and executed in JupyterLab (Version 3.6.1) on a DELL Precision workstation with the following specifications: Intel Xeon 5220R 24-Core CPU clocked at 2.2 GHz, 256 GB of RAM, 8 TB hard disk, running Ubuntu 20.04. The workstation was equipped with an NVIDIA Dual RTX A6000 Graphics Board (with NV Link) featuring 48 GB of video memory and 10,752 CUDA cores for each board. 
