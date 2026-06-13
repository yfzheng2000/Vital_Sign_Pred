# Vital_Sign_Pred

**Note: Two demo videos uploaded to: demo_video/ (illustrated below)**

Paper: Hybrid Neural Network Models to Estimate Vital Signs from Facial Videos
       https://www.mdpi.com/2673-7426/5/1/6

Related Paper: Continuous and contactless blood pressure monitoring using a hybrid neural network model based on facial video analysis
               https://doi.org/10.1117/12.3097753 (check it out from Subfolder: ./papers/)

Instruction to infer vital signs with the pre-trained models:

(1) download the test data file: 'Norm_30Frm_ValIdx250.npz'-- One sample (idx=250) from the test subset: X normalized to [-1,1], Y ground truth (not scaled). Note: Users are Not permitted to distribute or publish this data.

(2) download the pre-trained weights of 'Mdl_a': 'Mdl_a.weights.h5', 6.2GB -- cannot uploaded here due to its size. The downloading link for this weights file (manually copy/paste the following two parts together & remove spaces if any):  
https://drive.google.com  
/file/d/1rCS6hOCyaWdmr5u9yKQO7ilUBkBWr3go/view?usp=sharing

(3) 'hybrid_face_vital.ipynb': run this code in Jupyter Lab (Notebook) or in Google Colab to Predict Vital Signs from Facial Videos.

(4) Note: put the weights (.h5) file and test data file (.npz) in the same directory as this code. Code and files were Tested and Worked smoothly in both Google Colab with 15GB GPU, and Jupyter Lab with A6000 48GB GPU.

(5) Demo videos for HR, O2, BP estimation:

[https://github.com/yfzheng2000/Vital_Sign_Pred/blob/main/demo_video/Face2Vital-HR-O2_%202025-09-02_Cropped.mp4
](https://github.com/user-attachments/assets/749c8334-a1e5-484b-a357-ce137ec7a397)

[https://github.com/yfzheng2000/Vital_Sign_Pred/blob/main/demo_video/Face2Vital-BP_%202025-09-02_Cropped.mp4
](https://github.com/user-attachments/assets/0bb856af-bbd6-4f14-a542-9c898eb63269)

Nvidia A6000 GPU configuration for our experiments: 
All models were implemented using Python 3.9 and TensorFlow 2.19 (Keras 3), and executed in JupyterLab (Version 3.6.1) on a DELL Precision workstation with the following specifications: Intel Xeon 5220R 24-Core CPU clocked at 2.2 GHz, 256 GB of RAM, 8 TB hard disk, running Ubuntu 20.04. The workstation was equipped with an NVIDIA Dual RTX A6000 Graphics Board (with NV Link) featuring 48 GB of video memory and 10,752 CUDA cores for each board. 
