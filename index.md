## What is Channel Charting?

**Channel charting** learns a mapping from channel state information (CSI) to a so-called **channel chart** in which nearby datapoints indicate nearness in real space. In other words, the learned channel chart captures the spatial geometry of the transmitting user equipments (UEs), effectively encoding relative (or logical) UE locations. Channel charting is self-supervised as the mapping from CSI to the channel chart is learned only using a database of passively collected CSI information. Such a data-driven localization approach has the advantages of being scalable and avoiding reference location information, e.g., from global navigation satellite systems (GNSSs). The self-supervised nature of channel charting also avoids the need for line-of-sight (LoS) propagation conditions or (costly) measurement campaigns, while enabling the infrastructure basestations or access points to perform cognitive and predictive radio access network (RAN) tasks which are tied to UE location. 

### Typical Channel Charting Pipeline 

![channel charting pipeline](images/channel_charting_pipeline.png)

An infrastructure basestation (BS) or access point (AP) *passively* collects high-dimensional CSI (describing complex-valued frequency and time coefficients at possibly multiple antennas) from a large number transmitting UEs and/or UE locations. The BS or AP then generates CSI features, which describe large-scale fading properties contained in the collected CSI. Finally, dimensionality reduction (DR)-techniques are applied to the CSI-feature-database in order to learn a low-dimensional description which is the **channel chart**. The channel chart has the key properties that nearby points correspond to nearby locations in real space. 

* * *

## Publications

* C. Studer, S. Medjkouh, E. Gönültaş, T. Goldstein and O. Tirkkonen, "<a href="https://ieeexplore.ieee.org/abstract/document/8444621">Channel Charting: Locating Users Within  the Radio Environment Using Channel State Information</a>," IEEE Access, Vol. 6, pp. 47682-47698, Aug. 2018

## Patents

* C. Studer and O. Tirkkonen, "<a href="https://patents.google.com/patent/US10911168B2/en">Channel Charting in Wireless Systems</a>," U.S. Patent No. 10911168, Feb. 2021

## Software

* <a href="https://github.com/IIP-Group/ChannelCharting">Simple Channel Charting MATLAB Simulator</a>

* * *

**Important:** This website is maintained by the Integrated Information Processing (IIP) Group, led by <a href="mailto:studer@ethz.ch?subject=Channel Charting Repository">Prof. Christoph Studer</a>, in the <a href="https://ee.ethz.ch/">Department of Information Technology and Electrical Engineering</a> at <a href="https://ethz.ch/en.html">ETH Zürich</a>, Switzerland. In case you would like to **suggest** a publication, patent, or software link, then please contact  <a href="mailto:eg566@cornell.edu?subject=New Channel Charting Resource">Mr. Emre Gönültaş</a> and provide all the necessary details required to create an item in the above lists. Last updated March 30, 2021. 
