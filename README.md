# AQUAFace-V

AQUAFace-V extends age-invariant face verification from static image matching to video-based identity authentication. The framework first uses MTCNN to detect and align faces, selecting the highest-quality frontal image as the reference ID. Remaining AgeDB images are processed through LivePortrait to generate realistic video sequences containing pose variations, eye blinks, and facial expressions. AQUALR-guided adaptive margin learning emphasizes difficult age-gap and low-quality samples, preserving discriminative identity features under challenging conditions. For video verification, frame-level facial embeddings are extracted and aggregated using temporal feature fusion, where mean cosine similarity across the sequence suppresses motion-induced noise while retaining identity-consistent information, enabling robust age-invariant Video-vs-ID matching.

Base Paper: https://sadiqebrahim.github.io/AQUAFace/
