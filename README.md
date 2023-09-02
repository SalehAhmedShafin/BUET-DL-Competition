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
