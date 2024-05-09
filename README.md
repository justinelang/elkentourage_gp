This `README.md` file was generated on 2024-05-08 by Justine Lang

## GENERAL INFORMATION

1.  Title of the Project: Managing Human-Wildlife Interactions: Ecological and Financial Assessment of Elk Feedground Closure in Teton County

2.  Author Information

A. Primary Contact Information 
Name: Justine Lang; Role: Data Manager; Institution: Bren School of Environmental Science & Management, University of California, Santa Barbara; Email: justinelang@bren.ucsb.edu  

B. Alternate Contact Information 
Name: Katherine Aristi; Role: Project Manager; Institution: Bren School of Environmental Science & Management, University of California, Santa Barbara; Email: katherinearisti@bren.ucsb.edu

Name: Delores Chan; Role: Communications Manager; Institution: Bren School of Environmental Science & Management, University of California, Santa Barbara; Email: deloreschan@bren.ucsb.edu

Name: Samuel Desre; Role: Financial Manager; Institution: Bren School of Environmental Science & Management, University of California, Santa Barbara; Email: samueldesre@bren.ucsb.edu

3.  Date of data collection: 2023-04-03 - 2024-03-22

4.  Geographic location of data collection: Teton County, WY and the broader Greater Yellowstone Ecosystem, USA

5.  Information about funding sources that supported the collection of the data: No funding was acquired. 

## SHARING/ACCESS INFORMATION

1.  Licenses/restrictions placed on the data: No restrictions are placed on the data. 

2.  Links to publications that cite or use the data: Aristi, K., Chan, D, Lang, J., & Desre, S. (2024). Managing Human-Wildlife Interactions: Ecological and Financial Assessment of Elk Feedground Closure in Teton County [Master’s Thesis Equivalent, Bren School of Environmental Science & Management, University of California, Santa Barbara]. https://bren.ucsb.edu/projects/managing-human-wildlife-interactions-ecological-and-financial-assessment-elk-feedground 

3.  Links to other publicly accessible locations of the data: Related data used in this project are archived in Dryad: https://doi.org/10.5061/dryad.98sf7m0rx 

4.  Was data derived from another source? If yes, list source(s): 

A. Financial_Repercussions
- agcensus22.csv: Tabular data were pulled from the 2022 USDA Census of Agriculture (https://www.nass.usda.gov/Publications/AgCensus/2022/Full_Report/Volume_1,_Chapter_2_County_Level/Wyoming/st56_2_011_011.pdf) 
- fund_code.Rmd and quarantine_code.Rmd: Code was adapted from Python code by Ben Foster (bentfoster@gmail.com). Hay price and consumption parameters were informed by Selk, 2022 (https://www.drovers.com/news/beef-production/how-much-hay-will-cow-consume-estimate-your-winter-feed-needs), the National Integrated Drought Information System, 2022 (https://www.drought.gov/sites/default/files/2022-07/Western-Drought-Status-Update-July-2022.pdf), and the National Agriculture Statistics Service, 2022 (https://www.nass.usda.gov/Statistics_by_State/Wyoming/Publications/Brochures/Wyoming%20Hay%20Facts%202022.pdf)

B. Public_Comment

C. Transmission_Risk
- cattle_reactor_code_final.Rmd: Functions and most parameters were adapted from Kauffman et al., 2016 (https://doi.org/10.1016/j.prevetmed.2016.08.004). Current elk-cattle overlap was informed by the USDA Animal Health and Plant Inspection Service, 2023 (https://www.aphis.usda.gov/aphis/ourfocus/animalhealth/animal-disease-information/cattle-disease-information/tuberculosis-brucellosis-monthly-report). Jackson elk seroprevalence was informed by Merkle et al., 2017 (https://doi.org/10.1111/1365-2664.13022). Female elk proportion was informed by Eric Cole, USFWS (eric_cole@fws.gov)

5.  Recommended citation for the project: Lang, J., Aristi, K., Chan, D., & Desre, S. (2024). Managing Human-Wildlife Interactions: Ecological and Financial Assessment of Elk Feedground Closure in Teton County [GitHub Repository]. GitHub. https://github.com/justinelang/elkentourage_gp 

## DATA & FILE OVERVIEW

1.  File List: 

A. Financial_Repercussions
- agcensus22.csv: Teton County cattle census data pulled from the 2022 USDA Census of Agriculture
- fund_code.Rmd: functions to calculate brucellosis compensation fund size
- quarantine_code.Rmd: functions to calculate the cost of quarantining cattle under different brucellosis risk scenarios

B. Public_Comment
- specific Rmd or script name

C. Transmission_Risk
- cattle_reactor_code_final.Rmd: functions to calculate brucellosis transmission risk under different elk-to-cattle overlap and elk seroprevalence scenarios

2.  Relationship between files, if important:
- fund_code.Rmd uses agcensus22.csv
- cattle_reactor_code_final.Rmd output informs fund_code.Rmd and quarantine_code.Rmd input
- quarantine_code.Rmd output informs fund_code.Rmd input
- [public comment file names here]

## METHODOLOGICAL INFORMATION

1.  Description of methods used for collection/generation of data: All data used to inform parameters and code were pulled or adapted from literature and consultations with experts. See sources listed above. 

2.  Methods for processing the data:

A. Financial_Repercussions: Using different brucellosis risk scenarios (years between cattle cases) modeled with cattle_reactor_code_final.Rmd, quarantine_code.Rmd was run to calculate the cost of cattle quarantine based on cattle case frequency. This output was input into fund_code.Rmd to calculate the size of a brucellosis compensation fund in USD. See "Calculations for Change in Brucellosis Costs in Teton County" within the final report for additional methods and a table of parameters.  

B. Public_Comment: Public comments were read through and then analyzed for general sentiments and attitudes and ideas. Letters were also analyzed for ideas and suggestions that respondents offered. PDFs of the public comments were then read into [code name], where a sentiment analysis was performed using the NRC Word-Emotion Association Lexicon from Saif Mohammad and Peter Turney. See "Elk Feedground Public Sentiment Analysis" within the final report for additional methods.

C. Transmission_Risk: With different elk-cattle overlap and elk seroprevalence inputs (low, medium, high), cattle_reactor_code_final.Rmd was run to simulate brucellosis tranmission risk scenarios. Output is number of years between cattle reactors. See the markdown file and "Brucellosis Transmission Risk Model" within the final report for additional methods and a table of parameters. 

3.  Instrument- or software-specific information needed to interpret the data: \<include full name and version of software, and any necessary packages or libraries needed to run scripts\>

4.  People involved with sample collection, processing, analysis and/or submission: Kat Aristi, Delores Chan, Justine Lang, and Samuel Desre. 

## DATA-SPECIFIC INFORMATION FOR:

\[FILENAME\] \<repeat this section for each dataset, folder or file, as appropriate\>

1.  Number of variables:

2.  Number of cases/rows:

3.  Variable List: \<list variable name(s), description(s), unit(s)and value labels as appropriate for each\>

4.  Missing data codes: \<list code/symbol and definition\>

5.  Specialized formats or other abbreviations used:
