---
title: "Master's Thesis: Unsupervised Approaches for 4D Panoptic Segmentation in LiDAR Driving Scenes"
collection: publications
permalink: /publication/masters-thesis
excerpt: 'This work proposes, implements and evaluates an unsupervised approach for online 4D panoptic segmentation.'
date: 2025-01-04
venue: 'CTU Digital Library'
paperurl: 'http://hdl.handle.net/10467/109306'
citation: 'Jan Vlk (2025) &quot;Unsupervised Approaches for 4D Panoptic Segmentation in LiDAR Driving Scenes.&quot; http://hdl.handle.net/10467/122473.'
share: false
---

4D panoptic segmentation, which combines semantic and instance segmentation across LiDAR sequences, is crucial for enabling robust scene understanding in autonomous driving. Supervised methods rely on costly labeled datasets, limiting scalability across diverse driving scenarios. This thesis proposes FlowSeg4D, an unsupervised framework for online 4D panoptic segmentation that minimizes annotation requirements while achieving competitive performance. FlowSeg4D integrates unsupervised scene flow estimation with clustering techniques to ensure temporal consistency and accurate instance association, leveraging the WaffleIron model for semantic segmentation. Evaluated on SemanticKITTI, FlowSeg4D achieves LSTQ of 46.9 and association scores up to 73.0 for specific classes, rivaling supervised methods. Key findings highlight the inconsistent impact of scene flow and demonstrate strong generalization on out-of-distribution data, as evidenced by results on the PONE dataset. By advancing unsupervised 4D panoptic segmentation, this work contributes to scalable, cost-effective perception systems for safer autonomous driving.
BibTeX:

```
@inproceedings{Vlk2025FlowSeg4D,
title={Unsupervised Approaches for 4D Panoptic Segmentation in LiDAR Driving Scenes},
  author={Jan Vlk},
  year={2025},
  url={http://hdl.handle.net/10467/122473}
}
```
