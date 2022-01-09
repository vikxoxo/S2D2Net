# S2D2Net
The code for ImageNet CNN and CapsNet based hybrid model for steel defect recognition

Paper published in 2021 IEEE International Conference on Image Processing (ICIP), and availaible at https://ieeexplore.ieee.org/document/9506405

Kindly cite the paper if you find the study relevant, and useful.

BibTex: 
@INPROCEEDINGS{9506405,  author={Nath, Vikanksh and Chattopadhyay, Chiranjoy},  booktitle={2021 IEEE International Conference on Image Processing (ICIP)},   title={S2D2Net: An Improved Approach For Robust Steel Surface Defects Diagnosis With Small Sample Learning},   year={2021},  volume={},  number={},  pages={1199-1203},  doi={10.1109/ICIP42928.2021.9506405}}

Plain Text:
V. Nath and C. Chattopadhyay, "S2D2Net: An Improved Approach For Robust Steel Surface Defects Diagnosis With Small Sample Learning," 2021 IEEE International Conference on Image Processing (ICIP), 2021, pp. 1199-1203, doi: 10.1109/ICIP42928.2021.9506405.Abstract: Surface defect recognition of products is a necessary process to guarantee the quality of industrial production. This paper proposes a hybrid model, S2D2Net (Steel Surface Defect Diagnosis Network), for an efficient and robust inspection of the steel surface during the manufacturing process. The S2D2Net uses a pretrained ImageNet model as a feature extractor and learns a Capsule Network over the extracted features. The experimental results on a publicly available steel surface defect dataset (NEU) show that S2D2Net achieved 99.17% accuracy with minimal training data and improved by 9.59% over its closest competitor based on GAN. S2D2Net proved its robustness by achieving 94.7% accuracy on a diversity enhanced dataset, ENEU, and improved by 3.6% over its closest competitor. It has better, robust recognition performance compared to other state-of-the-art DNN-based detectors.URL: https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9506405&isnumber=9506009

Note: Stay Tuned, Code will be updated in due time. Kindly contact nath.2@iitj.ac.in for any help related to this paper, and result reproduction

NEU Data: https://www.kaggle.com/kaustubhdikshit/neu-surface-defect-database

ENEU Data: https://drive.google.com/drive/folders/1Aj4mI1WqKqpOkC36I1vpG2PFQU56DxSL?usp=sharing

Meanwhile one may use following repo (https://github.com/rccohn/NEU-Cluster) for histogram equalization, and size change to (224,224,3) of ENEU or NEU dataset images, and can also save extracted feature maps (e.g. VGG16 conv base feature maps having dimension [7,7,512]) for whole data (train, and test NEU as well as ENEU) using this repo.

Then one may learn/train a CapsNet using extracted feature maps of NEU train set, and can test the trained CapsNet over extracted feature maps of NEU test set, and whole ENEU.

For CapsNet implementation one may follow any good implementaion from GitHub. I followed https://github.com/XifengGuo/CapsNet-Keras

If still needs a help to reproduce the results, or some help in pipeline implementation on your own task. Kindly connect at nath.2@iitj.ac.in


