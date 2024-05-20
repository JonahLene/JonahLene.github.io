---
layout: project
type: project
image: img/MD5CollisionHash.png
title: "MD5 Collision Attack Lab"
date: 2024-05-10
published: true
labels:
  - Cybersecurity
  - MD5 Hash Algorithm
  - Collision Attack
  - SEED Labs
  - Ubuntu
  - Virtual Machine

summary: "The solo cybersecurity project involved a hands-on exploration of MD5 collision attacks, including generating hash collisions, understanding the properties of the MD5 algorithm, and creating executable files with identical hashes but different behaviors. This comprehensive learning experience reinforced the importance of adaptability and continuous learning in the dynamic field of cybersecurity."
---

<img class="img-fluid" src="../img/Screenshot%202024-05-20%20133427.png">

In the MD5 Collision Attack Lab, I got to delve into the intricacies of cryptographic hash functions, specifically focusing on the MD5 algorithm. The primary goal was to understand the importance of the collision-resistance property, which ensures that it’s computationally infeasible to find two different inputs producing the same hash value. Through this lab, I could see firsthand how vulnerabilities in hash functions like MD5 and SHA-1 can lead to significant security breaches, as demonstrated by real-world attacks.

In the first task, I generated two distinct files that shared the same MD5 hash using the md5collgen tool. This tool allowed me to provide a prefix for both files, and I verified that the outputs were different but had identical hash values using the diff and md5sum commands. This exercise vividly illustrated how two different files could be crafted to produce the same hash, highlighting the vulnerability of MD5 to collision attacks.

Next, I explored some fundamental properties of the MD5 algorithm. I designed an experiment to demonstrate that if two inputs produce the same hash, appending the same suffix to both results in outputs with the same hash. Using file concatenation commands, I confirmed this property, reinforcing my understanding of MD5's iterative process and the implications of its structure.

In the third task, I took on the challenge of creating two different executable files with the same MD5 hash. By working with binary data, I used a hex editor and the md5collgen tool to manipulate specific sections of compiled programs. This involved identifying and modifying particular bytes to create hash collisions while ensuring that the executables behaved differently. This task was a practical demonstration of how collision attacks can be applied, and it gave me valuable experience in working with binary files.

Finally, I tackled a more advanced scenario where two programs with the same MD5 hash had entirely different behaviors based on internal conditions. By manipulating arrays within the program's binary, I made one version execute benign code and the other execute malicious code. This task demonstrated how an attacker could potentially exploit the collision vulnerability to get a malicious program certified as benign. This scenario underscored the critical importance of collision-resistant hash functions in maintaining the integrity and security of software and data.


Lab Report: [MD5 Collision Attack Lab Report](https://docs.google.com/document/d/1-JAO1mbFJmnzzD4WO2j8pjnZzg9QdRZ-UGasOSRzGqQ/edit).
