# csiro-aos-object-detection
AWS and Gluon to analyze orange roughy data

Naming convention for fine tuned object detectors: 

[DATE]-[NETWORK].[DATATYPE].params

- VOC[side]MASTER == Original data from AOS in VOC format
- VOC[side]MERGE == Merged labels to ensure 100% overlap of organisms between runs/eliminate classes with few examples
- VOC[side]ALL == put all runs together into single image folder with seperate lists for each run. fascilitates experimenting with training on all OPs

Notes:
- 12/31 Combined all the runs into VOC[side]ALL. Deleted JPEGImages from VOC[side]MERGE to save storage space.