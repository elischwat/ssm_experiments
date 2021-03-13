# ssm_experiments
Python notebooks for modifying and analyzing Salish Sea Model (SSM) input and output files.

analyze_ssm_inputs.ipynb
* Analyze point source input data. Looks in depth at total nitrogen loading from individual rivers and waste water treatment plants (WWTPs).

analyze_ssm_inputs_with_modifications.ipynb
* Analyze point source input data. Calculates total nitrogen loading from rivers and WWTPs.

modify_ssm_inputs.ipynb
* Modify effluent concentration data for rivers and WWTPs. Allows you to set constant values for different water quality parameters and apply those values to every time step in the input dataset. Outputs a modified input file for us with the Salish Sea Model.

check_ssm_inputs.ipynb
* Informal testing for the modify_ssm_inputs.ipynb notebook. Opens up an input file and makes sure the right file lines and tokens were modified.

extract_ssm_outputs.ipynb
* Extract data from the ssm_station.out file output by the SSM. A limited number of sub-daily output variables are collected and saved to a csv.gz file to make analysis easier.

analyze_ssm_outputs.ipynb
* Analyze SSM outputs in the format output by the extract_ssm_outputs.ipynb notebook. Looks at maximum ammonium and nitrate, minimum dissolved oxygen, and dissolved oxygen time series. Multiple csv.gz files (such as those created from multiple different ssm_station.out files from different model runs) can be read into a single dataset and analyzed for comparison.
