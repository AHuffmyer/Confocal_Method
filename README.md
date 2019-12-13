{\rtf1\ansi\ansicpg1252\cocoartf1671\cocoasubrtf600
{\fonttbl\f0\froman\fcharset0
TimesNewRomanPS-BoldMT;\f1\froman\fcharset0
TimesNewRomanPSMT;\f2\froman\fcharset0 TimesNewRomanPS-ItalicMT; }
{\colortbl;\red255\green255\blue255;\red0\green0\blue0;}
{\*\expandedcolortbl;;\cssrgb\c0\c1\c1;}
\margl1440\margr1440\vieww14240\viewh12480\viewkind0 \deftab720
\pard\tx3006\pardeftab720\ri0\partightenfactor0

\f0\b\fs24 \cf0 Study: \f1\b0 \cf2 Evaluation of laser scanning confocal
microscopy as a method for characterizing reef-building coral tissue
thickness and Symbiodiniaceae fluorescence\cf0\
\pard\pardeftab720\ri0\partightenfactor0

\f0\b \cf0 Authors: \f1\b0 Huffmyer AS, SB Matsuda, AR Eggers, JD Lemus,
RD Gates\
 \f0\b Corresponding Author: \f1\b0 AS Huffmyer, ashuffmyer@gmail.com,
ashuff@hawaii.edu\
\
This study describes and evaluates the utility of laser-scanning
confocal microscopy to measure physiological condition (Symbiodiniaceae
fluorescence and depth of fluorescence) in reef-building corals. \f0\b  
\f1\b0\
 \f0\b \
Abstract: \f1\b0\
\
Predicting the sensitivity of reef-building corals to disturbance,
including bleaching, requires an understanding of physiological
responses to stressors, which may be limited by destructive sampling and
the capacity of common methodologies to characterize early life history
stages. We developed a new methodology using laser scanning confocal
microscopy (LSCM) to measure and track the physiological condition of
corals. In a thermal stress experiment, we used LSCM to track coral
condition during bleaching in adults and juveniles of two species,
\f2\i Montipora capitata \f1\i0 and \f2\i Pocillopora acuta \f1\i0 .
Depth of fluorescence in coral tissues provides a proxy measure of
tissue thickness while fluorescence of Symbiodiniaceae populations
relates to both population density and chlorophyll- content. In response
to thermal stress, here were significant shifts in tissue thickness and
Symbiodiniaceae fluorescence with differences in condition between life
stages. This method is particularly well-suited for detecting shifts in
physiological condition of living corals, especially in small juvenile
colonies.\
\
\
 \f0\b Data, Scripts, and Outputs: \f1\b0\
\
All data for analysis is contained in the Data folder. All analyses are
conducted in the Confocal\_Markdown\_Final.Rmd file with output of the
markdown file as Confocal\_Markdown\_Final.html. Running scripts in the
R Markdown file will produce data summary files into the Output folder
and final figures used in the manuscript will be generated in the
Figures folder.\
\
The Data folder contains data files necessary for analysis to be loaded
into the R Markdown script and are described below.\
\
Validations folder:\
\
'93AdultCoral\_SymbiontCellCounts.csv'94 - Symbiont cells in adult coral
tissues as measured on a hemocytometer.\
 '93Date'94 = date tissue sample was analyzed on a hemocytometer\
 '93Sample'94 = the species code and colony ID number sample was
collected from\
 '93Species'94 = species (MCAP = Montipora capitata, PVAR = Pavona
varians, PACU = Pocillopora acuta, PCOM = Porites compressa)\
 '93AreaCM'94 = surface area of tissue sample in cm\^2\
 '93TubeRep'94 = replicate aliquots of tissue slurry\
 '93TechRep'94 = technical replicate within tissue aliquot\
 '93Symbionts.cm2'94 = total symbiont cells per cm\^2 area of tissue\
\
'93AdultCoral\_DissectScopeThickness.csv'94 - Adult coral tissue
thickness measured on a dissecting microscope.\
 '93Tunic'94 = tunic ID corresponding to species and colony ID number\
 '93Tissue'94 = tissue type at location of measurement (colony, polyp,
or connecting tissue)\
 '93Thickness'94 = tissue thickness in microns\
\
'93AdultCoral\_ConfocalFluorescence.csv'94 - Adult coral symbiont
fluorescence as measured by LSCM\
 '93Sample'94 = sample ID corresponding to species and colony ID number\
 '93Species'94 = coral species\
 '93Tissue'94 = tissue type at location of measurement\
 '93Area'94 = surface area of measurement\
 '93Tissue.Intensity'94 = green/host tissue fluorescence intensity (not
used in this study)\
 '93Tissue.StDev'94 = standard deviation of fluorescence intensity of
host tissue\
 '93Symbiont.Intensity'94 = red/symbiont fluorescence intensity in area
of measurement\
 '93Symbiont.StDev'94 = standard deviation of fluorescence intensity of
symbiont\
\
'93AdultCoral\_ConfocalThickness.csv'94 - Adult coral depth of
fluorescence as measured by LSCM\
 '93Sample'94 = sample ID corresponding to species and colony ID number\
 '93Species'94 = coral species\
 '93Tissue'94 = tissue type at location of measurement\
 '93Slice'94 = replicate of slice analyzed within a sample 3D model\
 '93Location'94 = XY location of slice\
 '93Thickness'94 = tissue thickness in microns measured at three
locations on each slice\
\
Bleaching folder:\
\
'93Bleaching\_Chlorophyll\_Content.csv'94 - Chlorophyll content of
corals measured by spectrophotometry at the end of thermal stress
experiment\
 '93Sample'94 = sample ID corresponding to coral colony ID number\
 '93Colony'94 = colony ID number\
 '93Chla Mean'94 = mean value of chlorophyll a\
 '93Chla CV'94 = coefficient of variation of chlorophyll a\
 '93SurfaceArea'94 = surface area of sample determined by wax dipping in
cm\^2\
 '93Chla.SA'94 = Chlorophyll a content normalized to sample surface area
(cm\^2)\
\
'93Bleaching\_Scope\_Thickness.csv'94 - Tissue thickness of corals
measured on a dissecting microscope at the end of thermal stress
experiment\
 '93Sample'94 = sample ID corresponding to coral colony ID number\
 '93Colony'94 = colony ID number\
 '93Species'94 = coral species\
 '93LifeStage'94 = life stage of sample, either adult or juvenile\
 '93Treatment'94 = temperature treatment, either ambient or high\
 '93rep1'94 = tissue thickness measurement of tissue tunic\
 '93rep2'94 = tissue thickness measurement of tissue tunic\
 '93rep3'94 = tissue thickness measurement of tissue tunic\
 '93rep4'94 = tissue thickness measurement of tissue tunic\
 '93Thickness'94 = mean sample tissue thickness across replicates\
\
'93Bleaching\_Coral\_Color.csv'94 - Bleaching score by coral
pigmentation as a ratio of coral color to a white standard at the end of
thermal stress experiment\
 '93Timepoint'94 = timepoint, final indicates end of thermal stress
experiment\
 '93Sample'94 = sample ID corresponding to coral colony ID number\
 '93Colony'94 = colony ID number\
 '93Treatment'94 = temperature treatment, either ambient or high\
 '93Species'94 = coral species\
 '93LifeStage'94 = life stage of sample, either adult or juvenile\
 '93Black'94 = color value of black standard\
 '93White'94 = color value of white standard\
 '93Coral'94 = color value of coral sample from top view of sample\
 '93White-Black'94 = color value of white standard correcting for noise
in black standard\
 '93Coral-Black'94 = color value of coral correcting for noise in black
standard\
 '93Coral Percent White'94 = coral color value divided by white standard
(coral : white)\
\
'93Bleaching\_Confocal\_Fluorescence.csv'94 - Symbiodiniaceae
fluorescence values measured by LSCM on corals at the beginning and end
of thermal stress experiment\
 '93Day'94 = day of exposure in thermal stress experiment\
 '93Timepoint'94 = timepoint, either initial or final\
 '93Sample'94 = sample ID corresponding to coral colony ID number\
 '93Colony'94 = colony ID number\
 '93Treatment'94 = temperature treatment, either ambient or high\
 '93Species'94 = coral species\
 '93LifeStage'94 = life stage of sample, either adult or juvenile\
 '93Tissue.Intensity'94 = value of fluorescence intensity from host
tissues\
 '93Symbiont.Intensity'94 = value of fluorescence intensity from
Symbiodiniaceae\
\
'93Bleaching\_Confocal\_Thickness.csv'94 - Depth of fluorescence values
measured by LSCM on corals at the beginning and end of thermal stress
experiment\
 '93Day'94 = day of exposure in thermal stress experiment\
 '93Timepoint'94 = timepoint, either initial or final\
 '93Sample'94 = sample ID corresponding to coral colony ID number\
 '93Colony'94 = colony ID number\
 '93Treatment'94 = temperature treatment, either ambient or high\
 '93Species'94 = coral species\
 '93LifeStage'94 = life stage of sample, either adult or juvenile\
 '93Location'94 = XY location of slice in sample\
 '93Thickness'94 = value of depth of fluorescence in sample\
\
\
\
\
}
