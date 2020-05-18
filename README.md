# pcap2pic
该代码用以将CTU-13和ISOT-2010的pcap包转化为灰度图，作为深度学习模型的样本，进而实现僵尸网络的检测。需要首先使用pkt2flow(https://github.com/caesar0301/pkt2flow)将pcpa包按照五元组切割成流。

These codes are used to convert CTU-13 and ISOT-2010 pcap packages into grayscales to carry out botnet detection with deep learning. You may use pkt2plow(https://github.com/caesar0301/pkt2flow) to split pcap packages into flow groups ahead.

# usage
Jupyter notebooks used in this project converts ISOT-2010 and CTU-13 files into grayscales and hdf5 to input a ResNet50 model.

The two compressed files contains all the botnet flows transffered into graycales in CTU-13, and all normal flows processed into grayscales in ISOT-2010, which both have mapping from name to label in csv files.
