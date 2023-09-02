# BUET-DL-Competition

Bengali is the fifth most spoken of all native languages worldwide. After completing the month-long signature Deep Learning competition on Bengali Automatic Speech Recognition (ASR) last year, we at the Department of Computer Science and Engineering, BUET now focus on another computational challenge. This year again, in partnership with Bengali.AI, we welcome participants to attend the DL Sprint 2.0 and play around with the first multi-domain large Bengali Document Layout Analysis Dataset: BaDLAD, as a part of BUET CSE Fest 2023.

For training the model, we will use a subset of the BaDLAD dataset contributed by our co-host, Bengali.AI. The details of the dataset can be found in this paper

This competition is open to all, not only for undergraduates. Anyone from any institution can participate.
However, in the spirit of fairness, all students from BUET CSE18 (the organizing batch) are disallowed from participating.

**About the Dataset:**

The dataset for this competition comprises about 34,000 Bengali documents annotated using polygon boundaries and rectangular bounding boxes. These documents range from newspaper articles, official documents, notices, and government gadgets to novels, comics, magazines, and even liberation war records.

The annotations specify the regions in these documents that fall into 4 classes -

Paragraph

Text Box

Image

Table

Your task is to design a deep learning pipeline that takes in a document image (.png) and predicts bounding polygon segments (masks) for each occurrence of the classes mentioned above in the input image.

**Data Details**

There are 20,365 training and 13,000 test images. The train and test images can be found in in badlad/images/ directory, whereas the labels for the train dataset can be found in badlad/labels/ directory.

**Predictions**

Your model should predict the masks for bounding polygons in each image. A mask is a 2D matrix corresponding to each input image pixel. The contents of each pixel position can be 0 or 1. If the pixel position is marked 0, then that position corresponds to the background category, no paragraph, text box, image, or table exists at that pixel. This mask is called a binary mask because of its content. Each prediction category (paragraph, text box, image, table) has a binary mask for each image. For example, image 846df66a-610e-4356-b369-6788885a0dc5.png has 4 binary masks, for each existing category - that predict where in the image, that specific category occurs.

Paper link-

@article{shihab2023badlad,
  title={BaDLAD: A Large Multi-Domain Bengali Document Layout Analysis Dataset},
  author={Shihab, Md Istiak Hossain and Hasan, Md Rakibul and Emon, Mahfuzur Rahman and Hossen, Syed Mobassir and Ansary, Md Nazmuddoha and Ahmed, Intesur and Rakib, Fazle Rabbi and Dhruvo, Shahriar Elahi and Dip, Souhardya Saha and Pavel, Akib Hasan and others},
  journal={arXiv preprint arXiv:2303.05325},
  year={2023}
}


