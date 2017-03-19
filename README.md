# Comparison of different reconstruction algorithms and calibration scans for a multi band sequence

The subject was instructed to move their eyes and blink throughout the duration of the reconstructed sequence (but kept their eyes closed for one of the calibration scans - see below). Multiband factor was set to 8. The images were 
reconstructed using different algorithms and calibration scans:

1. [1D-GRAPPA with built in (internal) calibration scan - eyes open](file:///D:/scratch/slice_leakage/mriqc/out/reports/sub-pilot1_task-rest_rec-old_bold.html) 
1. [SS-GRAPPA with built in (internal) calibration scan - eyes open](file:///D:/scratch/slice_leakage/mriqc/out/reports/sub-pilot1_task-rest_SSGInternalEyesOpen-old_bold.html) 
1. [SS-GRAPPA with high SNR (single band) calibration scan - eyes open](file:///D:/scratch/slice_leakage/mriqc/out/reports/sub-pilot1_task-rest_rec-SSGExternalCalEyesOpen_bold.html) 
1. [SS-GRAPPA with high SNR (single band) calibration scan - eyes closed](file:///D:/scratch/slice_leakage/mriqc/out/reports/sub-pilot1_task-rest_rec-SSGExternalCalEyesClosed_bold.html) 
1. [Quality metrics comparison](https://cdn.rawgit.com/chrisfilo/slice_leakage/033e8b20/reports/bold_group.html)

Switching from 1D-GRAPPA to SS-GRAPPA slightly reduced the leakage (and only in the white matter - see slices 40-42). Using a fully sampled single band claibration scan almost completely removed leakage. Data reconstructed using eyes closed calibration scan had slightly higher tSNR and SNR, but otherwise the difference between the two was minimal.
