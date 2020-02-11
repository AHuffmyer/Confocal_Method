
**Study:** Evaluation of laser scanning confocal microscopy as a method for characterizing reef-building coral tissue thickness and Symbiodiniaceae fluorescence

**Authors:** Huffmyer AS, SB Matsuda, AR Eggers, JD Lemus, RD Gates

**Corresponding Author:** AS Huffmyer, ashuffmyer@gmail.com

This study describes and evaluates the utility of laser-scanning confocal microscopy to measure physiological condition (Symbiodiniaceae fluorescence and depth of fluorescence) in reef-building corals.

**Abstract:**

Predicting the sensitivity of reef-building corals to disturbance, including bleaching, requires an understanding of physiological responses to stressors, which may be limited by destructive sampling and the capacity of common methodologies to characterize early life history stages. We developed a new methodology using laser scanning confocal microscopy (LSCM) to measure and track the physiological condition of corals. In a thermal stress experiment, we used LSCM to track coral condition during bleaching in adults and juveniles of two species, _Montipora capitata_ and _Pocillopora acuta_. Depth of fluorescence in coral tissues provides a proxy measure of tissue thickness while Symbiodiniaceae population fluorescence relates to both population density and chlorophyll-a content. In response to thermal stress, there were significant shifts in tissue thickness and Symbiodiniaceae fluorescence with differences between life stages. This method is particularly well-suited for detecting shifts in physiological condition of living corals in laboratory studies, especially in small juvenile colonies. 

**Data, Scripts, and Outputs:**

All data for analysis is contained in the Data folder. All analyses are conducted in the Confocal_Markdown_Final.Rmd file with output of the markdown file as Confocal_Markdown_Final.html. Running scripts in the R Markdown file will produce data summary files into the Output folder and final figures used in the manuscript will be generated in the Figures folder. 

The Data folder contains data files necessary for analysis to be loaded into the R Markdown script and are described below. 

**Validations folder:** 

“AdultCoral_SymbiontCellCounts.csv” - Symbiont cells in adult coral tissues as measured on a hemocytometer. 

“Date” = date tissue sample was analyzed on a hemocytometer

“Sample” = the species code and colony ID number sample was collected from

“Species” =  species (MCAP = Montipora capitata, PVAR = Pavona varians, PACU = Pocillopora acuta, PCOM = Porites compressa)

“AreaCM” =  surface area of tissue sample in cm^2

“TubeRep” = replicate aliquots of tissue slurry

“TechRep” = technical replicate within tissue aliquot 

“Symbionts.cm2” = total symbiont cells per cm^2 area of tissue



“AdultCoral_DissectScopeThickness.csv” - Adult coral tissue thickness measured on a dissecting microscope. 

“Tunic” = tunic ID corresponding to species and colony ID number

“Tissue” = tissue type at location of measurement (colony, polyp, or connecting tissue)

“Thickness” = tissue thickness in microns



“AdultCoral_ConfocalFluorescence.csv” - Adult coral symbiont fluorescence as measured by LSCM 

“Sample” = sample ID corresponding to species and colony ID number

“Species” = coral species

“Tissue” = tissue type at location of measurement

“Area” =  surface area of measurement 

“Tissue.Intensity” = green/host tissue fluorescence intensity (not used in this study)

“Tissue.StDev” = standard deviation of fluorescence intensity of host tissue

“Symbiont.Intensity” = red/symbiont fluorescence intensity in area of measurement

“Symbiont.StDev” = standard deviation of fluorescence intensity of symbiont 



“AdultCoral_ConfocalThickness.csv” - Adult coral depth of fluorescence as measured by LSCM

“Sample” = sample ID corresponding to species and colony ID number

“Species” = coral species 

“Tissue” = tissue type at location of measurement

“Slice” = replicate of slice analyzed within a sample 3D model

“Location” = XY location of slice

“Thickness” = tissue thickness in microns measured at three locations on each slice



**Bleaching folder:** 

“Bleaching_Chlorophyll_Content.csv” - Chlorophyll content of corals measured by spectrophotometry at the end of thermal stress experiment

“Sample” = sample ID corresponding to coral colony ID number

“Colony” = colony ID number

“Chla Mean” = mean value of chlorophyll a

“Chla CV” = coefficient of variation of chlorophyll a

“SurfaceArea” = surface area of sample determined by wax dipping in cm^2

“Chla.SA” = Chlorophyll a content normalized to sample surface area (cm^2)



“Bleaching_Scope_Thickness.csv” - Tissue thickness of corals measured on a dissecting microscope at the end of thermal stress experiment

“Sample” = sample ID corresponding to coral colony ID number

“Colony” = colony ID number

“Species” = coral species 

“LifeStage” = life stage of sample, either adult or juvenile

“Treatment” = temperature treatment, either ambient or high

“rep1” = tissue thickness measurement of tissue tunic

“rep2” = tissue thickness measurement of tissue tunic

“rep3” = tissue thickness measurement of tissue tunic

“rep4” = tissue thickness measurement of tissue tunic

“Thickness” = mean sample tissue thickness across replicates 



“Bleaching_Coral_Color.csv” - Bleaching score by coral pigmentation as a ratio of coral color to a white standard at the end of thermal stress experiment

“Timepoint” = timepoint, final indicates end of thermal stress experiment

“Sample” = sample ID corresponding to coral colony ID number

“Colony” = colony ID number

“Treatment” = temperature treatment, either ambient or high

“Species” = coral species 

“LifeStage” = life stage of sample, either adult or juvenile

“Black” = color value of black standard

“White” = color value of white standard

“Coral” = color value of coral sample from top view of sample

“White-Black” = color value of white standard correcting for noise in black standard

“Coral-Black” = color value of coral correcting for noise in black standard

“Coral Percent White” = coral color value divided by white standard (coral : white)



“Bleaching_Confocal_Fluorescence.csv” - Symbiodiniaceae fluorescence values measured by LSCM on corals at the beginning and end of thermal stress experiment

“Day” = day of exposure in thermal stress experiment

“Timepoint” = timepoint, either initial or final

“Sample” = sample ID corresponding to coral colony ID number

“Colony” = colony ID number

“Treatment” = temperature treatment, either ambient or high

“Species” = coral species 

“LifeStage” = life stage of sample, either adult or juvenile

“Tissue.Intensity” = value of fluorescence intensity from host tissues

“Symbiont.Intensity” = value of fluorescence intensity from Symbiodiniaceae



“Bleaching_Confocal_Thickness.csv” - Depth of fluorescence values measured by LSCM on corals at the beginning and end of thermal stress experiment

“Day” = day of exposure in thermal stress experiment

“Timepoint” = timepoint, either initial or final

“Sample” = sample ID corresponding to coral colony ID number

“Colony” = colony ID number

“Treatment” = temperature treatment, either ambient or high

“Species” = coral species 

“LifeStage” = life stage of sample, either adult or juvenile

“Location” = XY location of slice in sample 

“Thickness” = value of depth of fluorescence in sample

 
