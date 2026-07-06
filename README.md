## UAV_2024
Radar data of UAVs Spring/Summer 2024

# Cite as
S. Kearney and S. Z. Gurbuz, "Physics-Guided Deep Neural Networks for Radar-Based UAV Recognition in Different Environments With No Prior In Situ Data," in IEEE Transactions on Aerospace and Electronic Systems, vol. 62, pp. 9875-9891, 2026, doi: 10.1109/TAES.2026.3685229.

# Abstract
Classifying uncrewed aerial vehicle (UAV) radar micro-Doppler
signatures with deep neural networks (DNNs) suffers a degradation
in performance when there is a difference in the distribution of training
and test data due to the differences in clutter backscatter and signal-tointerference-plus-noise ratio (SINR) of different environments. This
is further exacerbated in low-SINR samples in which the helicopter
motor rotation (HERM) line characteristic of UAV blade rotations
becomes only faintly visible. As HERM lines are a critical feature
enabling the recognition and discrimination of various types of UAVs,
this article addresses the twofold challenge of 1) how to accurately
synthesize HERM lines in training data for UAV classification and
2) how to enhance recognition performance in previously unseen
different environments, especially when the SINR is low. Toward these
aims, we propose a physics-guided approach in which a semantic
segmentation network trained only using low-fidelity computer aided
design (CAD)-models of UAVs is integrated into the discriminator of
a generative adversarial network (GAN) for training data synthesis,
and on the front end of a DNN for classification. Our results show that
physics-guided semantic segmentation improves the representation of
HERM lines in GAN-synthesized samples and enables improved classification of low-SINR samples exhibiting HERM lines when no prior
in situ data at that SINR are used during training. Consequently, our
approach provides a way of enhancing UAV recognition performance
in different operational environments, from which it is often difficult
to obtain training data prior to deployment.
