This README.txt file was generated on 20181113 by Albert Presto


-------------------
GENERAL INFORMATION
-------------------


1. Title of Dataset:


Mobile AMS (aerosol mass spectrometer) datasets collected as part of CACES.



2. Author Information

    Corresponding Author Contact Information
        Name: Albert Presto
           Institution: Carnegie Mellon University
           Address: 5000 Forbes Ave, Pittsburgh, PA 15213
           Email: apresto@andrew.cmu.edu

	Author Contact Information
        Name:Peishi Gu
           Email: peishigu@gmail.com

	Author Contact Information
        Name:Rishabh Shah
           Email: rshah6192@gmail.com

---------------------
DATA & FILE OVERVIEW
---------------------

Directory of Files
   A. Filename: Pittsburgh_AMS_Mobile_2016_2017.xlsx    
      This file contains mobile AMS data collected in Pittsburgh in 2016-2017. It is identical to the dataset used in Gu et al (ES&T, 2018, DOI: 10.1021/acs.est.8b03833). Data are reported for total PM mass, PM components, and organic aerosol components determined from positive matrix factorization (PMF). The file also contains data for concurrent measurements of particulate black carbon (BC), and gaseous pollutants (CO, CO2, NO, NO2, NOx).  


        
   B. Filename: README_AMS_Mobile.txt       
      Short description: ReadMe file



-----------------------------------------------------------
DATA DESCRIPTION FOR: Pittsburgh_AMS_Mobile_2016_2017.xlsx 
-----------------------------------------------------------
1. Number of variables: 47


2. Number of cases/rows: 16393


3. Missing data codes:
        NaN (blank cell) -- missing gas data for CO2, CO, NO, NO2, NOx


4. Variable List

    A. Name: OBJECTID
       Description: Column A. Counter for data point number in the series.


    B. Name: datetime
       Description: Column B. Timestamp of AMS data.

	C. Name: run_index
	Description: Column C. Global index of sample numbers logged by the instrument.

	D. Name: Longitude
	Description: Column D. Mean longitude measured during each sample.

	E. Name: latitude
	Description: Column E. Mean latitude measured during each sample.

	F. Name: Elevation
	Description: Column F. Mean elevation above sea level (meters) measured during each sample.

	G. Name: hour
	Description: Column G. Hour of the day.

	H. Name: CO2
	Description: Column H. CO2 concentration measured in ppm. 

	I. Name: CO
	Description: Column I. CO concentration measured in ppb.

	J. Name: NO
	Description: Column J. NO concentration measured in ppb.

	K. Name: NO2
	Description: Column K. NO2 concentration measured in ppb.

	L. Name: NOx
	Description: Column L. NOx (=NO + NO2) measured in ppb.

	M. Name: matlab_date
	Description:  Column M. matlab-encoded date value for use in background correction of BC.

	N. Name: month
	Description: Column N. Month of the year.

	O. Name: PageName
	Description: Column O. Corresponds to "page" in GIS used for spatial aggregation of data.

	P. Name: PageNumber
	Description: Column P. Corresponds to "page" in GIS used for spatial aggregation of data.

	Q. Name: Population
	Description: Column Q. Population in the specific page used for aggregating this data point.

	R. Name: VMT_daily
	Description: Column R. Daily vehicle miles traveled (VMT) in the specific page.

	S. Name: VMT_daily_truck
	Description: Column S. Daily VMT contributed by diesel trucks in each page.

	T. Name: Restaurant_Count
	Description: Column T. Number of restaurants in the page.

	U. Name: Road_length_meter
	Description: Column U. Road length, in meters, in the page.

	V. Name: MOOOA
	Description: Column V. Concentration of MOOOA (more oxidized oxidized organic aerosol) from PMF analysis. Units: microgram/m^3.

	W. Name: LOOOA
	Description: Column W. Concentration of LOOOA (more oxidized oxidized organic aerosol) from PMF analysis. Units: microgram/m^3.

	X. Name: BBOA
	Description: Column X. Concentration of BBOA (biomass burning organic aerosol) from PMF analysis. Units: microgram/m^3.

	Y. Name: COA
	Description: Column Y. Concentration of COA (cooking organic aerosol) from PMF analysis. Units: microgram/m^3.

	Z. Name: HOA
	Description: Column Z. Concentration of HOA (hydrocarbon-like organic aerosol) from PMF analysis. Units: microgram/m^3.

	AA. Name: Residual
	Description: Column AA. Residual from the PMF fit. Units: microgram/m^3

	AB. Name: Org
	Description: Column AB. Organic aerosol concentration in microgram/m^3.

	AC. Name: OrgRB
	Description: Column AC. Regional background organic aerosol concentration in microgram/m^3.

	AD. Name: OrgLocal
	Description: Column AD. Local organic aerosol concentration (Org - OrgRB).

	AE. Name: SO4
	Description: Column AE. Particulate sulfate concentration.

	AF. Name: SO4RB
	Description: Column AF. Regional background sulfate concentration.

	AG. Name: SO4Local
	Description: Column AG. Local sulfate concentration.

	AH. Name: NO3
	Description: Column AH. Particulate nitrate concentration.

	AI. Name: NO3RB
	Description: Column AI. Regional background nitrate concentration.

	AJ. Name: NO3Local
	Description: Column AJ. Local nitrate concentration.

	AK. Name: NH4
	Description: Column AK. Particulate ammonium concentration.
	
	AL. Name: NH4RB
	Description: Column AL. Regional background ammonium concentration.

	AM. Name: NH4Local
	Description: Column AM. Local ammonium concentration.

	AN. Name: BC
	Description: Column AN. Black carbon (BC) concentration.

	AO. Name: BCRB
	Description: Column AO. Regional background BC concentration.

	AP. Name: BCLocal
	Description: Column AP. Local BC concentration.

	AQ. Name: Weight
	Description: Column AQ. The sampling rate differs in some cases. Some samples were collected at 60 sec resolution, others at 30 sec, and most at 20 sec. In the process of spatial joining, the weight of each sample must be taken into consideration. In the column “weight” lists the relative weight of each sample, 3 is 60 sec samples, 1.5 for 30 sec and 1 for 20 sec. 

	AR. Name: Site
	Description: Column AR. Each sample is also assigned a "site" that corresponds to the neighborhood where the sample was collected.

	AS. Name: Period
	Description: Column AS. Column “period” is a dummy variably that denote which period of day was this sample collected. “1” stands for morning (5-10), “2” stands for mid-day (11-16), “3” stands for evening (17-22) and “4” stands for overnight (23-4).

	AT. Name: Season
	Description: Column AT.  “1” is summer (8,9), “2” is fall (11) and “3” is winter (12, 1 and 2).

	AU. Name: Type
	Description: Column AU. “Type” is the land-use classification based on the GIS covariates (VMT and restaurant count). Type 1 has 0 VMT and 0 restaurant, Type 2 has 0 VMT and >0 restaurant, Type 3 has >0 VMT and 0 restaurant, Type 4 has >0 VMT and >0 restaurant.

---------------------------------------------------------------------
METHODOLOGICAL INFORMATION FOR: Pittsburgh_AMS_Mobile_2016_2017.xlsx 
---------------------------------------------------------------------

#
# Software: If specialized software(s) generated your data or
# are necessary to interpret it, please provide for each (if
# applicable): software name, version, system requirements,
# and developer.
#

1. Software-specific information:
<create a new entry for each qualifying software program>

Name: SQUIRREL
Version: 1.61
Source Repository URL: http://cires1.colorado.edu/jimenez-group/ToFAMSResources/ToFSoftware/#Analysis2

Name: PIKA
Version: 1.21F
Source Repository URL: http://cires1.colorado.edu/jimenez-group/ToFAMSResources/ToFSoftware/#Analysis2

Name: AMS PMF tool
Version: 3.04 A
Source Repository URL: http://cires1.colorado.edu/jimenez-group/wiki/index.php/PMF-AMS_Analysis_Guide#PMF_Evaluation_Tool_Software
Application notes: The PMF factors are based on the 5 factor solution with fpeak=-0.4. Sensitivity analysis of the PMF factorization is found in the supporting information of Gu et al (2018, DOI: 10.1021/acs.est.8b03833).



#
# Equipment: If specialized equipment generated your data,
# please provide for each (if applicable): equipment name,
# manufacturer, model, and calibration information. Be sure
# to include specialized file format information in the data
# dictionary.
#

2. Equipment-specific information:

See Methods section of Gu et al (2018, DOI: 10.1021/acs.est.8b03833).





#
# Dates of Data Collection: List the dates and/or times of
# data collection.
#

3. Date of data collection (single date, range, approximate date) <suggested format YYYYMMDD>: 20160808 - 20170217




