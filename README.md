# AGToLightM_TrainingData
All datasets in this repository are processed dataset, generated from original satellite observations and lightning measurements.No raw observational data are included.

# Data Storage Structure Documentation

This document describes the data storage structure, including satellite data and lightning data organization.

## Overall Directory Structure

```
Data/
├── EVB_Singel/                    # Satellite raw band data and lightning labels
│   ├── HasPointsIn1Hour/         # Lightning label data (1-hour rolling window)
│   ├── EVB0390_IMGs/             # EVB 0390 band images
│   ├── EVB0620_IMGs/             # EVB 0620 band images
│   ├── EVB0700_IMGs/             # EVB 0700 band images
│   ├── EVB0740_IMGs/             # EVB 0740 band images
│   ├── EVB0855_IMGs/             # EVB 0855 band images
│   ├── EVB1040_IMGs/             # EVB 1040 band images
│   ├── EVB1230_IMGs/             # EVB 1230 band images
│   └── EVB1330_IMGs/             # EVB 1330 band images
│
├── EVB_Difference/                # Band difference data (parent directory of EVB_Singel)
│   ├── 0620-0740/                # Difference between 0620 and 0740 bands
│   ├── 1040-0855/                # Difference between 1040 and 0855 bands
│   └── 1230-1040/                # Difference between 1230 and 1040 bands
│
├── EVB_TimeDiff/                 # Temporal difference data
│   ├── EVB1040_Diff/             # Temporal difference of EVB1040 band
│   └── EVB1230_Diff/             # Temporal difference of EVB1230 band
│
└── EVB_BandDiff_TimeDiff/        # Band difference temporal difference data
    ├── EVB_BandDiff_TimeDiff_1040-0855/  # Temporal difference of 1040-0855 band difference
    └── EVB_BandDiff_TimeDiff_1230-1040/  # Temporal difference of 1230-1040 band difference
```
## Note
The processed datasets provided in this repository take the East China region as a representative example.
Due to file size limitations, only the full-day data from June 1, 2025 are uploaded as a representative data example.
