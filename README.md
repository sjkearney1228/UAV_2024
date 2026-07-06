# UAV_2024
Radar data of UAVs Spring/Summer 2024

## Dataset
For the purpose of this article, radar data were collected
on a variety of UAVs using the TI AWR2243 single-chip
77- to 81-GHz radar. This FMCW radar was operated with
a waveform utilizing the full 4-GHz bandwidth and a pulse
repetition frequency (PRF) of 6.4 kHz, as defined in Table I.
The radar was placed 1.5 m above the ground and operated
for increments of 30 s per sample. The UAVs contained in
this dataset are described in Section III-A, and then, the
method for processing the dataset for use in deep learning
is explained in Section III-B.
Utilizing the FMCW radar, data were collected on five
UAVs, which varied in terms of size, number of propellers,
and length of propellers. Each of the UAVs is displayed
in Fig. 1 and described in Table II, where it can be seen
that the target set consists of: two Hexacopters and three
Quadcopters. The smaller of the two hexacopters has a
propeller length of 230 mm and a span of 0.86 m, while
the larger hexacopter has a propeller length of 230 mm and
a span of 1.31 m. Among the quadcopters, the propeller
lengths utilized were 147, 230, and 230 mm, which each had
a corresponding span of 0.24, 0.55, and 1.4 m, respectively.
These five UAVs were chosen to create a rich dataset whose
radar returns should be uniquely distinguishable but will
provide some overlap in distribution among the UAVs with
the same number of propellers.
This dataset was collected over two different collection
periods to increase the breadth of UAVs utilized for this
work, as defined in Table III. The first set of data was
collected on the small hexacopter and the medium-sized
quadcopter. Each of these UAVs was flown around 5 m from
the radar while hovering in an open field as well as with a
car and then a tree [as shown in Fig. 2(a)] each 5 m behind
the UAV and therefore 10 m from the radar to increase
the variability in environmental noise in our dataset. Ten
samples per a background environment were collected on
each of these UAVs. During this collection, the weather
was generally fair with a temperature around 24◦ C and
a wind speed of no larger than 8 kph. During the second
collection, the large hexacopter as well as the smaller and
larger quadcopters was utilized. As shown in Fig. 2(b), each
of the UAVs was flown around 5 m from the radar while
hovering in an open field with eight samples collected for
each quadcopter and three samples for the hexacopter given
battery time constraints when flying. For this collection, the
weather was hotter with a temperature around 33◦ C and a
similar wind speed as the other data collection of no larger
than 8 kph.

## Download Dataset
[UAV Dataset](https://example.com)

## Cite As
S. Kearney and S. Z. Gurbuz, "Physics-Guided Deep Neural Networks for Radar-Based UAV Recognition in Different Environments With No Prior In Situ Data," in IEEE Transactions on Aerospace and Electronic Systems, vol. 62, pp. 9875-9891, 2026, doi: 10.1109/TAES.2026.3685229.

## Abstract
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
