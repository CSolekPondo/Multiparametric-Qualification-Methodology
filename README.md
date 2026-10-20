# Multiparametric Qualification Methodology

Browser-based application implementing a multiparametric methodology for the post-process qualification of FFF-manufactured PEEK and TPU components through complementary FTIR, TGA and DSC characterization.

The tool compares experimental characterization data from a reference specimen and an evaluated specimen using material- and technique-specific descriptors.

## Workflow

1. **Material selection**  
   Select the polymer to be evaluated: **PEEK** or **TPU**. The application automatically adapts the analysis parameters to the selected material.

2. **Node 1 – FTIR**  
   Upload the FTIR datasets for the reference and evaluated specimens. The application processes the spectra and evaluates changes in chemical integrity through a material-specific degradation descriptor.

3. **Node 2 – TGA**  
   Upload the TGA datasets for the reference and evaluated specimens. The thermogravimetric curves are processed to evaluate changes in the thermal degradation behavior of the material.

4. **Node 3 – DSC**  
   Upload the DSC datasets for the reference and evaluated specimens. The application evaluates the relevant thermal transitions during the heating–cooling–heating cycle and compares their evolution between both conditions.

5. **Final assessment**  
   Click **Run evaluation** to process the data and display the calculated descriptors, relative variations and graphical results. FTIR and TGA are classified as **ACCEPTABLE**, **RE-EXAMINE** or **NOT ACCEPTABLE** according to the selected thresholds, while DSC provides complementary information on the thermal response. The final qualification outcome integrates the FTIR and TGA classifications.

## Input data

The application accepts experimental characterization datasets in Excel format (`.xlsx` or `.xls`).

For each characterization technique, two datasets are required:

- **Reference specimen**
- **Evaluated specimen**

The application automatically identifies and processes the relevant experimental data contained in the uploaded files.

The experimental datasets used to generate and validate the results reported in the associated publication are provided separately as Supporting Information.

## How to use

1. Download `MultiparametricQualificationMethodology_V1.html`.
2. Open the file in a web browser.
3. Select **PEEK** or **TPU**.
4. Upload the reference and evaluated datasets for FTIR, TGA and DSC.
5. For **FTIR**, review or modify the spectral ranges used for descriptor calculation.
6. For **DSC**, review or modify the temperature ranges used to evaluate the relevant thermal transitions.
7. Review or modify the qualification thresholds if required.
8. Click **Run evaluation**.
9. Review the calculated descriptors, relative variations, plots and final qualification outcome.

Experimental files are processed locally in the user's browser and are not uploaded to an external server.

## Official version and integrity check

The only official distribution of this software is this repository (see **Releases** for versioned downloads).
To verify that your copy of the file is the original, unmodified version, compare its SHA-256 checksum:

| File | Version | SHA-256 |
|---|---|---|
| `MultiparametricQualificationMethodology_V1.html` | v1.0 | `099ea71b52a1d387dee32ed975fed6954f6c3d530c0416a2abc7ae053323383b` |

- **Windows (PowerShell):** `Get-FileHash MultiparametricQualificationMethodology_V1.html -Algorithm SHA256`
- **macOS / Linux:** `shasum -a 256 MultiparametricQualificationMethodology_V1.html`

If the checksum does not match, the file has been modified and is not the authors' official version.

## Contact

For questions regarding the application, please contact: csolek@ind.uned.es

## License

Copyright © 2026 Claudia Solek, Jorge Crespo-Sánchez, Sergio Fuentes del Toro,
Jorge Ayllón, Mariaenrica Frigione, Ana M. Camacho, Juan Rodríguez-Hernández
and Álvaro Rodríguez-Prieto.

This software can be **freely downloaded and used** for research, academic and
educational purposes, **provided that the associated work is cited** (see below).

Modification or redistribution of the source code, in whole or in part, and any
commercial use require prior written permission from the authors
(contact: **csolek@ind.uned.es**). See the [LICENSE](LICENSE) file for details.

### How to cite

Any use of this software or of results obtained with it must cite:

> C. Solek, J. Crespo-Sánchez, S. Fuentes del Toro, J. Ayllón, M. Frigione,
> A. M. Camacho, J. Rodríguez-Hernández, Á. Rodríguez-Prieto.
> *From Characterization to Qualification: An Integrated Multiparametric
> Methodology for Additively Manufactured Polymer Components.*
> Manuscript submitted, 2026.
> Software: https://github.com/CSolekPondo/Multiparametric-Qualification-Methodology

The citation will be updated with the journal reference and DOI upon publication.
You can also use the **"Cite this repository"** button on the right-hand side of this page.
