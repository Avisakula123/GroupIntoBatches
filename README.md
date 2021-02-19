# Apache_Beam_python-GroupIntoBatches
# Rohith Avisakula [![](https://img.shields.io/badge/Github-Avisakula123)](https://github.com/Avisakula123)
## Sub-topic : GroupIntoBatches
- I have worked on GroupIntoBatches for dataset [gas_retail.csv](https://www.kaggle.com/mruanova/us-gasoline-and-diesel-retail-prices-19952021)
- [My Google Colab Notebook on GroupIntoBatches](https://github.com/Rajeshwari-Rudra/apache_beam-python/blob/main/GroupIntoBatches.ipynb)
- [Demonstration Video link](https://app.vidgrid.com/view/3zL17htuXTRE)


## Prerequisites
- Python
- Apache beam
- Google Colaboratory

## Commands Used 
- Install apache beam using the below command.
```
pip install apache-beam
```
- Next install the dependencies required using below command.
```
!pip install apache-beam[gcp,aws,test,docs]
```

- The command that lists all the files.
```
! ls
```
- First sign in to google drive account and google colab with same credentials and upload .csv file to google drive account.
- Import .csv file into google colab.
```
# Code to read csv file into colaboratory:
!pip install -U -q PyDrive
from pydrive.auth import GoogleAuth
from pydrive.drive import GoogleDrive
from google.colab import auth
from oauth2client.client import GoogleCredentials
```
```
# Autheticate E-Mail ID
auth.authenticate_user()
gauth = GoogleAuth()
gauth.credentials = GoogleCredentials.get_application_default()
drive = GoogleDrive(gauth)
```
```
# Get File from Drive using file-ID
# Get the file
downloaded = drive.CreateFile({'id':'1b73yN7MjGytqSP5wimYAQmtByOvGGe8Y'}) # replace the id with id of file you want to access
downloaded.GetContentF
```
- Command for result
```
! cat results.txt-00000-of-00001
```

## Screenshots for commands

- For installation of apache beam.

![](https://github.com/Rajeshwari-Rudra/apache_beam-python/blob/main/rohith-images/install.PNG)

- For installing required dependencies and libraries.

![](https://github.com/Rajeshwari-Rudra/apache_beam-python/blob/main/rohith-images/dependencies.PNG)

- Program for GroupIntoBatches.

![](https://github.com/Rajeshwari-Rudra/apache_beam-python/blob/main/rohith-images/code1.PNG)

- For importing file into colobaratory.

![](https://github.com/Rajeshwari-Rudra/apache_beam-python/blob/main/rohith-images/code.PNG)

- For display of list of files.

![](https://github.com/Rajeshwari-Rudra/apache_beam-python/blob/main/rohith-images/list.PNG)

- For output of the file.

![](https://github.com/Rajeshwari-Rudra/apache_beam-python/blob/main/rohith-images/output.PNG)

## References

* [kaggle](https://www.kaggle.com/mruanova/us-gasoline-and-diesel-retail-prices-19952021)
* [Apache](https://beam.apache.org/documentation/transforms/python/aggregation/groupintobatches)
* [Colab](https://colab.research.google.com/notebooks/intro.ipynb)
