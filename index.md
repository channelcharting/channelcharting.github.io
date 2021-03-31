## What is Channel Charting?

**Channel charting** learns a mapping from channel state information (CSI) to a so-called **channel chart** in which nearby datapoints indicate nearness in real space. In other words, the learned channel chart captures the spatial geometry of the transmitting user equipments (UEs), effectively encoding relative (or logical) UE locations. Channel charting is self-supervised as the mapping from CSI to the channel chart is learned only using a database of passively collected CSI information. Such a data-driven localization approach has the advantages of being scalable and avoiding reference location information, e.g., from global navigation satellite systems (GNSSs). The self-supervised nature of channel charting also avoids the need for line-of-sight (LoS) propagation conditions or (costly) measurement campaigns, while enabling the infrastructure basestations or access points to perform cognitive and predictive radio access network (RAN) tasks which are tied to UE location. 

### Typical Channel Charting Pipeline 

![channel charting pipeline](images/channel_charting_pipeline.png)

An infrastructure basestation (BS) or access point (AP) *passively* collects high-dimensional CSI (describing complex-valued frequency and time coefficients at possibly multiple antennas) from a large number transmitting UEs and/or UE locations. The BS or AP then generates CSI features, which describe large-scale fading properties contained in the collected CSI. Finally, dimensionality reduction (DR)-techniques are applied to the CSI-feature-database in order to learn a low-dimensional description which is the **channel chart**. The channel chart has the key property that nearby points correspond to nearby locations in real space. 

* * *

## Publications

2018 

* C. Studer, S. Medjkouh, E. Gönültaş, T. Goldstein, and O. Tirkkonen, "<a href="https://ieeexplore.ieee.org/abstract/document/8444621">Channel Charting: Locating Users Within  the Radio Environment Using Channel State Information</a>," IEEE Access, Vol. 6, pp. 47682-47698, Aug. 2018

* J. Deng, S. Medjkouh, N. Malm, O. Tirkkonen, and C. Studer, "<a href="https://www.research-collection.ethz.ch/handle/20.500.11850/461322">Multipoint Channel Charting for Wireless Networks</a>," 52nd Asilomar Conference on Signals, Systems, and Computers, Oct. 2018

2019 

* T. Ponnada, J. Al-Tous, O. Tirkkonen, and C. Studer, "<a href="https://www.research-collection.ethz.ch/handle/20.500.11850/461386">An Out-of-Sample Extension for Wireless Multipoint Channel Charting</a>," Intl. Conference on Cognitive Radio Oriented Wireless Networks, June 2019

* P. Huang, O. Castañeda, E. Gönültaş, S. Medjkouh, O. Tirkkonen, T. Goldstein, and C. Studer, "<a href="https://arxiv.org/abs/1908.02878">Improving Channel Charting with Representation-Constrained Autoencoders</a>," IEEE 20th Intl. Workshop on Signal Processing Advances in Wireless Communications (SPAWC), July 2019

* E. Lei, O. Castañeda, O. Tirkkonen, T. Goldstein, and C. Studer, "<a href="https://arxiv.org/abs/1909.13355">Siamese Neural Networks for Wireless Positioning and Channel Charting</a>," 57th Annual Allerton Conference on Communication, Control, and Computing (Allerton), Sep. 2019

2020

* C. Geng, J. Huang, and J. Langerman, "Multipoint Channel Charting with Multiple-Input Multiple-Output Convolutional Autoencoder," IEEE/ION Position, Location and Navigation Symposium (PLANS), Apr. 2020, <a href="https://ieeexplore.ieee.org/document/9109875">paywall link</a>

* P. Agostini, Z. Utkovski, and S. Stańczak, "Channel Charting: An Euclidean Distance Matrix Completion Perspective," IEEE Intl. Conference on Acoustics, Speech and Signal Processing (ICASSP), May 2020, <a href="https://ieeexplore.ieee.org/abstract/document/9053639">paywall link</a>

* P. Kazemi, H. Al-Tous, C. Studer, and O. Tirkkonen, "<a href="https://acris.aalto.fi/ws/portalfiles/portal/61183483/SNR_Prediction_in_Cellular_Systems_based_on_Channel_Charting.pdf">SNR Prediction in Cellular Systems based on Channel Charting</a>," IEEE Eighth Intl. Conference on Communications and Networking (ComNet), Oct. 2020

* P. G. Burguera, "<a href="https://aaltodoc.aalto.fi/bitstream/handle/123456789/97603/master_Garau_Burguera_Pere_2020.pdf?sequence=1">Logical Radio Maps for User Localization in a Real Outdoor Radio Environment</a>," M.S. Thesis report, Aalto University, Finland, Nov. 2020

* J. Pihlajasalo, M. Koivisto, J. Talvitie, S. Ali-Löytty, M. Valkama, "Absolute Positioning with Unsupervised Multipoint Channel Charting for 5G Networks," IEEE 92nd Vehicular Technology Conference (VTC2020-Fall), Nov. 2020, <a href="https://ieeexplore.ieee.org/document/9348571">paywall link</a>

* H. Al-Tous, T. Ponnada, C. Studer, and O. Tirkkonen, "<a href="https://www.research-collection.ethz.ch/handle/20.500.11850/452594">Multipoint Channel Charting-Based Radio Resource Management for V2V Communications</a>," EURASIP Journal on Wireless Communications and Networking, Dec. 2020

* P. Ferrand, A. Decurninge, L. G. Ordoñez, and M. Guillaud, "<a href="https://arxiv.org/abs/2005.12242">Triplet-Based Wireless Channel Charting</a>," IEEE Global Communications Conference (GLOBECOM), Dec. 2020

* L. Ribeiro, M. Leinonen, D. Djelouat, and M. Juntti, "Channel Charting for Pilot Reuse in mMTC with Spatially Correlated MIMO Channels,"  IEEE Globecom Workshops, Dec. 2020, <a href="https://ieeexplore.ieee.org/abstract/document/9367434">paywall link</a>

## Patents

* C. Studer and O. Tirkkonen, "<a href="https://patents.google.com/patent/US10911168B2/en">Channel Charting in Wireless Systems</a>," U.S. Patent No. 10911168, Feb. 2021

## Software

* <a href="https://github.com/IIP-Group/ChannelCharting">Simple Channel Charting MATLAB Simulator</a>

* * *

**Important:** This website is maintained by the Integrated Information Processing (IIP) Group, led by <a href="mailto:studer@ethz.ch?subject=Channel Charting Repository">Prof. Christoph Studer</a>, in the <a href="https://ee.ethz.ch/">Department of Information Technology and Electrical Engineering</a> at <a href="https://ethz.ch/en.html">ETH Zürich</a>, Switzerland. In case you would like to **suggest** a publication, patent, or software link, then please contact  <a href="mailto:eg566@cornell.edu?subject=New Channel Charting Resource">Mr. Emre Gönültaş</a> and provide all the necessary details required to create an item in the above lists. Also note that we do *no longer* include resources that are behind a paywall. Last updated March 31, 2021. 
