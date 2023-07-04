# GOD_stimuli_annotations

## Summary
This repository shares the caption annotations of the 1200 training stimulus images used in the following KamitaniLab represetative papers. 

1. Horikawa, T., & Kamitani, Y. (2017). Generic decoding of seen and imagined objects using hierarchical visual features. Nature Communications, 8, 15037. https://doi.org/10.1038/ncomms15037
    - Github: [KamitaniLab/GenericObjectDecoding](https://github.com/KamitaniLab/GenericObjectDecoding)
2. Shen, G., Horikawa, T., Majima, K., & Kamitani, Y. (2019). Deep image reconstruction from human brain activity. PLOS Computational Biology, 15(1), 1006633. https://doi.org/10.1371/journal.pcbi.1006633
    - Github: [KamitaniLab/DeepImageReconstruction](https://github.com/KamitaniLab/DeepImageReconstruction)
3. Horikawa, T., & Kamitani, Y. (2022). Attention modulates neural representation to render reconstructions according to subjective appearance. Communications Biology, 5(1), 34. https://doi.org/10.1038/s42003-021-02975-5
    - Github: [KamitaniLab/End2EndDeepImageReconstruction](https://github.com/KamitaniLab/End2EndDeepImageReconstruction)

Caption data and category information are stored in *.jsonl. Please see [example.ipynb](example.ipynb) for detailed data usage.

```python
df = pd.read_json("data/ImageNetTraining_captions.jsonl", orient="records", lines=True)
display(df)
```
```
	image_id	category_id	captions
0	n01518878_10042	n01518878	[A brown and tan ostridge walking near a metal...
1	n01518878_12028	n01518878	[The head of an ostridge looking over a metal ...
2	n01518878_14075	n01518878	[A brown ostridge with its beak open walking i...
3	n01518878_14910	n01518878	[An ostrich walks across a dirt road towards g...
4	n01518878_5958	n01518878	[An ostrich standing in a field with trees beh...
...	...	...	...
1195	n13111881_28475	n13111881	[A small bonsai tree sits in the dirt in a sma...
1196	n13111881_6054	n13111881	[Miniature manicured trees on display table ou...
1197	n13111881_6560	n13111881	[Young woman watering her home plants joyfully...
1198	n13111881_7817	n13111881	[A bonsai tree in a bowl near a red wall., A s...
1199	n13111881_9170	n13111881	[A bonsai tree with gnarly white branches and ...
1200 rows × 3 columns
```


## Collection method for caption data
The caption data was collected in 2018 using Amazon Mechanical Turk (AMT), a crowdsourcing service. We use the following two worker filtering when collecting captions.
1. Masters has been granted.
2. HIT Approval Rate (%) for all Requesters' HITs greater than 95.

## About test image captions
As mentioned above, the annotation data for test images is not publicly available. This is to prevent the data from being crawled. If you wish to be shared the test image captions, please contact us separately via email (kaminitalab@gmail.com). Please ensure not to place the shared captions in public locations.


## About the sharing of fMRI data and stimulus image data
The stimulus image itself cannot be shared due to copyright problems. If you would like to need the data, so please contact us from [here](https://forms.gle/ujvA34948Xg49jdn9).
fMRI data is open to the public on figshare, etc. Please see the github repository of the above representative paper for details.
