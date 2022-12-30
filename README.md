# ChildhoodCancerDataInitiative-CCDI_to_dbGaP
This script will take data from a CCDI submission manifest, and create the Subject Consent, Subject Sample Mapping and Sample Attribute files specifically for a CCDI project.

To run the script on a complete [CCDI validated submission template](https://github.com/CBIIT/ccdi-model/tree/main/metadata-manifest), run the following command in a terminal where R is installed for help.

```
Rscript --vanilla CCDI_to_dbGaP.R --help
```

```
Usage: CCDI_to_dbGaP.R [options]

CCDI_to_dbGaP v2.0.0

This script will take a validated CCDI Submission Template and create a dbGaP submission for a consent 1 (GRU) study.

If a previous submission for the phs_id already exists, that file can be presented (-s) during the creation to make an updated file for that phs_id.


Options:
	-f CHARACTER, --file=CHARACTER
		A validated dataset file based on the template CCDI_submission_metadata_template (.xlsx)

	-s CHARACTER, --previous_submission=CHARACTER
		A previous dbGaP submission directory from the same phs_id study.

	-h, --help
		Show this help message and exit
```
