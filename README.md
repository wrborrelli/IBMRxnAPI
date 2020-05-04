# IBM Rxn API Mathematica Wrapper

This API wrapper simplifies the use of IBM Rxn for chemistry capabilities in Mathematica.

## Installation

Download the source code from the IBMRxn_RawCode file or IBMRxn_wDemo for the code plus a demonstration of its uses. 


## Usage
Below you will find a table outlining the capabilities of the function along with the necessary input and input types necessary for each action.
Request | Action | Inputs | Input Type 
------- | ------ | -------| ---------- 
new project | Creates a new project. | Request, Project Name | String, String
new prediction | Creates a new prediction. | Request, Reactants List, Project ID | String, List of Images/Strings, String
new retrosynthesis| Creates a new retrosynthesis. | Request, Project ID, Product Molecule List | String, String, List of Image/String
more predictions | Gets all predictions for a previous prediction. | Request, Project ID, Prediction ID | String, String, String
recover prediction | Recovers the results from a previous prediction. | Request, Prediction ID | String, String
recover retrosynthesis | Recovers the results from a previous retrosynthesis. | Request, Retrosynthesis ID | String, String
stored projects | Lists all stored projects, with project IDs. | Request | String
all project attempts | Lists all attempts within a project. | Request, Project ID | String, String
queue status | Gets retrosynthesis queue status information. | Request | String

All calls to the function are formatted with a string request specifying the action you would like to do, followed by the requisite inputs specified in the table above:
```bash
rxn["request", input___] 
```
## Support
Any support related inquiries may be directed to wborrelli@fordham.edu. 

## Authors and Acknowledgement
Dr. Joshua Schrier, Kim B. and Stephen E. Bepler Chair Professor of Chemistry at Fordham University, was immensely helpful in all aspects of this project. 
