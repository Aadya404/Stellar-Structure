Discovering Stellar Structure with Unsupervised Machine Learning 

This project explores whether meaningful stellar structure can be discovered purely from physical measurements, without using predefined labels or astrophysical rules. Instead of treating machine learning as
This work uses unsupervised learning to analyse, interpret, and test the stability of structures in real stellar data.



Astronomical objects are often classified using human-defined categories such as star types or spectral classes. If a machine is only given raw physical properties of stars, will structure naturally emerge 
from the data? The goal is to understand if stellar organisation is inherently encoded in physical features, which features are most critical for preserving that structure. 

Methods Used


Principal Component Analysis (PCA)
To examine whether a linear structure exists in a reduced-dimensional space.

K-Means Clustering
To test whether stars can be grouped automatically based on similarity, without labels.

Autoencoder Neural Network (PyTorch)
To learn a nonlinear latent representation of stellar data through compression and reconstruction.

Feature Removal Experiments
One physical feature is removed at a time to study how latent structure degrades under information loss.

Silhouette Score Analysis
To quantitatively evaluate cluster separation and support visual observations.

Label Visualization
Known star types are applied after training to assess alignment between learned structure and astrophysical categories.



Key Findings

Stellar structure emerges clearly from physical measurements even without labels.

Temperature and absolute magnitude play dominant roles in preserving separability.

Luminosity and radius provide overlapping, supportive information.

Using all features does not always yield the clearest structure, highlighting measurement redundancy.

The autoencoder’s latent space aligns closely with known star types, despite never being trained on labels.

These results suggest that stellar organisation is not an artefact of classification but an inherent property of the underlying physical features.

