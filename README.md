This is a repo for demonstraighting using Git for collaboration and learning how to utilize techniques learned in the 2016 June Software/Data Carpentry Workshop
This comes with data incase the datastore causes issues

### Git Collaborating
1. Groups member A, go to: https://github.com/tempu/scw_june_capstone_data.git
2. Fork the repo
3. Go to "Settings" -> "Collaborators" -> search for group member B's git username and click their name, then click "Add Collaborator"
4. Group member B, accept the invite in the email that went to the email you signed up to Github with.

### Commandline - Atmosphere Set-Up:
1. Clone the group/class repo
   1. git clone "URL_TO_GROUP_MEMBER_A_REPO"

2. Navigate to your group folder
    1. Group Member A make a scripts directory (mkdir) and then make a script (touch command) in that directory use Git commands to add, commit, and push (may need to do Git push origin master) the file you just made
    2. Groups member B do Git pull and make sure you now have a new file made by group member A.

3. Explore the data!

4. Group member A, pull

5. Group member A, open Jupyter notebook
   1. Group member A, Open the scrip
   2. Group member A, Annotate the script
   3. Group member A, Initial script

6. Make a figure with subplots A and B

###Tips
import pandas as pd
from matplotlib import pyplot as plt
%matplotlib inline

df = pd.read_csv('data_location')
df = df[df['column_name'] == something]

df['column_name'].dropna()

df['column_name'].hist()

new_df = df[[something, something, etc.]]

df.plot(x = 'something', y = 'something2', kind = 'type of plot')
url:
http://pandas.pydata.org/pandas-docs/stable/generated/pandas.DataFrame.plot.html

