--------------------------------------------------------------------------------
# LAG-1 - Learning, Attention, and Gaze 1
A free and open source category learning simulator written in MATLAB
--------------------------------------------------------------------------------

Version 1.0

Written by Jordan Barnes, Mark Blair, Calen Walshe and Paul Tupper at
Simon Fraser University and University of Texas, CPS.

GPL license.

## OVERVIEW

LAG-1 is a simple package that can be run from Matlab or compiled and run as a
standalone application.

You can download the latest version of LAG-1 from the git repository at:

https://github.com/SFU-Cognitive-Science-Lab/LAG-1


## INSTALLATION

Clone or decompress the archive in a folder of your choice and add this folder to to your MATLAB path. 

LAG-1 requires a Matlab installation, available for Windows, Mac OSX and Linux, or the installation of Matlab runtime libraries which are available here:

http://www.mathworks.com/products/compiler/mcr/

LAG-1, as first committed, has been tested on versions of Matlab dating as far back as 2007.


## QUICK START

* Begin by defining a category structure in experimentConfig.txt (and in several random spots as experiment specific conditions until cleaned up). 

* Set the desired values of parameter_source.txt

* Call the model using several different options:


	### Example usage

	**Default options**

	[accuracy, category, fixOrder, subjectNumber, Duration, recordSaccStart, recordSaccEnd, endFit, wtHist, accuracyLevels, Responses, ResponseDist] = TwoDSimulator(varargin)

	**Specific category structure** 
	* 1 = ET3
	* 2 = SSHRC_IF 
	* 3 = 5/4
	* 7 = Simple blocking structure

	[accuracy, category, fixOrder, subjectNumber, Duration, recordSaccStart, recordSaccEnd, endFit, wtHist, accuracyLevels, Responses, ResponseDist] = TwoDSimulator(1)

 	**Specific category structure and learning type** 
 	
	* 1 = corrective Hebbian association
	* 2 = only correct Hebbian association 
	* 3 = unsupervised decoupling of chosen answer with features 
	* 4 = unsupervised decoupling of chosen answer with features and coupling of alternative features with alternative categories.

	[accuracy, category, fixOrder, subjectNumber, Duration, recordSaccStart, recordSaccEnd, endFit, wtHist, accuracyLevels, Responses, ResponseDist] = TwoDSimulator(3,1)

## Note: expect 


## Agenda

Integration with Cosivina based pupil model with reinforcement learning

