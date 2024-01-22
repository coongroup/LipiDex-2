# LipiDex-2

### Software tools for liquid chromatography-mass spectrometry (LC-MS) lipidomics


### [Download](https://github.com/coongroup/LipiDex-2/releases/latest)

## Features and improvements
- **Library Generator:** Spectral library creation with *in silico* fragmentation.
   - **NEW:**
      - Support for MSn tree-based fragmentation, glycolipids, lipopeptides,
      - Simplified interface for for designing complex lipid classes
- **Spectrum Searcher:** Spectral library matching for identifying lipids from MS2 and MS3+ spectra
  - **NEW:**
    - Support for thermo .raw files
    - Parameters for RT filtering, MSn intensity threshold, PPM or Thomson mass error, and more
- **Peak Finder:** Lipid identification from a peak table
  - **NEW:**
     - Support for Compound Discoverer 3.3
     - Direct reading of Compound Discoverer .cdResult files, avoiding intermediate conversion to `.csv` peak table
- **Lipid Spectral Annotator** uses Spectrum Searcher MS2 and MS3+ spectral matches and annotates fragment peaks
- **NEW:** Degreaser Quality Control module allows for automated validation of lipid identifications and features using 6 pieces of evidence:
  - Effective carbon number versus retention time modeling (ECN vs. RT)
  - Dilution series linear dynamic range modeling
  - Biosample quantitations within linear range
  - Spectral match validation for all matches in the lipid feature
  - Replicate quality control samples' percent relative standard deviation (%RSD) with run order
  - Compound Discoverer's Peak Quality Factors (PQF) 

- **IMPROVED:** Results are filtered on 7 criteria to boost confidence in your identifications and quantitation

## Getting started
[Download the .zip file](https://github.com/coongroup/LipiDex-2/releases/latest), extract onto your computer and run LipiDex2.exe

Instructions are found in the [LipiDex 2 Wiki](https://github.com/coongroup/LipiDex-2/wiki) (WiP)

All LipiDex 2 modules are stand-alone and pass .csv results files through the pipeline. However Peak Finder requires [Compound Discoverer version 3.3](https://www.thermofisher.com/us/en/home/industrial/mass-spectrometry/liquid-chromatography-mass-spectrometry-lc-ms/lc-ms-software/multi-omics-data-analysis/compound-discoverer-software.html) .cdResult files as input for the peak table.

## Installing 

LipiDex 2 is a stand-alone executable program and does not require any installation.

.NET 7.0 is required. Your operating system will automatically prompt you to install them when you run LipiDex2.exe.



## Legacy LipiDex 1 
While no longer supported, LipiDex 1 is still available at https://github.com/coongroup/LipiDex 





