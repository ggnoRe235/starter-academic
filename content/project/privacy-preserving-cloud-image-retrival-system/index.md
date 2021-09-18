---
title: Privacy preserving cloud image retrival system
date: 2021-03-09T06:55:41.731Z
summary: >-2
  

    **Feb. 2020 - June. 2020**

  Followed up and improved a recent research about encrypted image retrieval system working on the cloud that could preserve user privacy.

    **Brief introduction of system:**

  * This system aims to solve the problem that in a cloud image retrieval system, cloud server could analyse user's requests and damage user privacy.

  * This system uses compressed binary CNN fully connected layer outputs to represent image features, and uses the distance among image features as the classification basis to generate a tree for retrieval. By encrypting the tree and user's requests with random matrix, cloud server can only use encrypted features to calculate distance between user's request and tree nodes during the retrieval process, and thus the system can preserve user privacy.


  **Completed improvements:**


  * Because the original system's tree generation process only merges nodes with high similarity, the subtrees of the generated tree may have obvious height differences, and it will leads to low accuracy since the features of nodes with small depth in the tree will become vague. By involving new threshold and check process, the system will get a chance to merge nodes with low similarity at the right time. Experiments show that the accuracy of the modified system is 8\% higher than that of the original system on average, and when more categories of images are used, the accuracy gap between the modified system and the original system is more obvious.

  * The original system's retrieval process will only pick one node which has the smallest distance with user's request at each level, so the original system doesn't perform well when there are similar nodes at the same level. By involving more (Experiments shows that the maximum of 3 nodes perform the best) similar nodes into consideration, modified system could reach higher accuracy.


  **Further improvements:**


  * It is inevitable that the features of nodes will become more vague during the tree generation process, and it will get worse if there are more categories of images involved, so that using tags during the tree generation process may achieve higher accuracy and it can also simplify the retrieval process.
draft: false
featured: false
tags:
  - ml
  - sec
  - crypt
external_link: a
links: []
image:
  filename: featured
  focal_point: Smart
  preview_only: false
---
  **Feb. 2020 - June. 2020**

Followed up and improved a recent research about encrypted image retrieval system working on the cloud that could preserve user privacy.

  **Brief introduction of system:**

* This system aims to solve the problem that in a cloud image retrieval system, cloud server could analyse user's requests and damage user privacy.
* This system uses compressed binary CNN fully connected layer outputs to represent image features, and uses the distance among image features as the classification basis to generate a tree for retrieval. By encrypting the tree and user's requests with random matrix, cloud server can only use encrypted features to calculate distance between user's request and tree nodes during the retrieval process, and thus the system can preserve user privacy.

**Completed improvements:**

* Because the original system's tree generation process only merges nodes with high similarity, the subtrees of the generated tree may have obvious height differences, and it will leads to low accuracy since the features of nodes with small depth in the tree will become vague. By involving new threshold and check process, the system will get a chance to merge nodes with low similarity at the right time. Experiments show that the accuracy of the modified system is 8\% higher than that of the original system on average, and when more categories of images are used, the accuracy gap between the modified system and the original system is more obvious.
* The original system's retrieval process will only pick one node which has the smallest distance with user's request at each level, so the original system doesn't perform well when there are similar nodes at the same level. By involving more (Experiments shows that the maximum of 3 nodes perform the best) similar nodes into consideration, modified system could reach higher accuracy.

**Further improvements:**

* It is inevitable that the features of nodes will become more vague during the tree generation process, and it will get worse if there are more categories of images involved, so that using tags during the tree generation process may achieve higher accuracy and it can also simplify the retrieval process.