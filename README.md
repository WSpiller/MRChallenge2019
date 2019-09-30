# MRChallenge2019

The `MRChallenge2019` R package provides necessary data and documentation for the 2019 Mendelian Randomization (MR) Conference data challenge.

The MR Data Challenge is an opportunity to explore and develop innovative approaches to causal inference using a rich source of genetic association data taken from Kettunen et al (1).

At a glance, these data comprise information on 150 SNPs and their association with

1. 118 lipid fraction traits (including HDL and LDL cholesterol)
2. Health outcomes (including type II Diabetes and stroke)

Researchers attending the upcoming 2019 Mendelian randomization conference in Bristol from July 17th-19th are encouraged to make use of all (or any part) of these data to Illustrate new methodology and to compare or explain existing methods as part of an oral or poster presentation.  

A special conference session is being planned to showcase all of the analyses attempted. Individuals will be encouraged to share software for transparency, with awards being given for innovation and reproducible research.  A key aim of the session will be to bring together methodologists and statisticians with experts from medicine, epidemiology and biological science, who will help to comment on and debate the results.

Further information on the specifics of the data challenge session will be released in the near future, including a set of challenge questions that individuals can choose to address in their analysis.

Please circulate widely among your research group and peers if planning to attend the conference, and encourage them to take part

 We look forward to seeing you in Bristol in the summer. Further information on the MR conference is available at https://www.mendelianrandomization.org.uk/.

## Installation

To install `MRChallenge2019` directly from the GitHub repository, first make sure you have the `remotes` package installed:

    install.packages("remotes")

Then the `MRChallenge2019` package can be installed using:

    library(remotes)
    install_github("WSpiller/MRChallenge2019", build_opts = c("--no-resave-data", "--no-manual"), build_vignettes = TRUE)
    
To update the package just run the `remotes::install_github("WSpiller/MRChallenge2019", build_opts = c("--no-resave-data", "--no-manual"), build_vignettes = TRUE)` command again.

Note that the change from previously running `install_github("WSpiller/MRChallenge2019",build_vignettes=T)` is a consequence of using the newer `devtools 2.0.1`.

## Description

The `MRChallenge2019` package contains two data frames, and a document describing the data and aims of the data challenge:

1. The data frame `Challenge_dat` contains summary data for the estimated associations between 118 metabolite risk factors and 150 genetic variants, with metabolite information quantified using nuclear magnetic resonance (NMR) spectroscopy metabolomics. The data also includes information on 7 outcomes; age-related macular degeneration, alzheimers's disease, type 2 diabetes, Ischemic stroke, large artery stroke, cardioembolic stroke, and small vessel stroke.

2. The data frame `NMRA_dat` contains the abbreviation, full name, overall heritability of the trait, and classification of each NMR trait.

3. Running the command `vignette("challenge")` will display a document giving a detailed description of the data and broad aims of the data challenge.


## Citation

For this challenge we used summary data previously published in Kettunen et al (1), originating from the Global Lipids Genetics (2), International AMD Genomics (3), DIAGRAM (4), and MEGASTROKE (4) consortia.

1. Kettunen J, Demirkan A, Würtz P, et al. Genome-wide study for circulating metabolites identifies 62 loci and reveals novel systemic effects of lpa. Nature communications [Internet]. 2016 March;7:11122. Available from: http://europepmc.org/articles/PMC4814583

2. Willer C, Schmidt E, Sengupta S, et al. Discovery and refinement of loci associated with lipid levels. Nature Genetics. Nature Publishing Group; 2013 Nov;45(11):1274–1285. 

3. Fritsche LG, Igl W, Bailey JNC, et al. A large genome-wide association study of age-related macular degeneration highlights contributions of rare and common variants. Nature genetics [Internet]. 2016 February;48(2):134—143. Available from: http://europepmc.org/articles/PMC4745342

4. Mahajan A, Taliun D, Thurner M, et al. Fine-mapping type 2 diabetes loci to single-variant resolution using high-density imputation and islet-specific epigenome maps. Nature Genetics. 2018 Oct;50. 

5. Malik R, Chauhan G, Traylor M, et al. Multiancestry genome-wide association study of 520,000 subjects identifies 32 loci associated with stroke and stroke subtypes. Nature genetics [Internet]. 2018 April;50(4):524—537. Available from: http://europepmc.org/articles/PMC5968830

## Acknowledgments

The majority of data formatting for this data challenge was provided by Verena Zuber and the Department of Epidemiology and Biostatistics, Imperial College London. Documentation has been adapted by the MRC Integrative Epidemiology Unit, University of Bristol for use in the 2019 MR Conference. The MR Conference will be held at Bristol from July 17th to July 19th, and more information can be found at https://www.mendelianrandomization.org.uk/. 

## License

This project is licensed under GNU GPL v2.




