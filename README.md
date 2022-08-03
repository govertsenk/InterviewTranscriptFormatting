# Interview Transcript Formatting
This Jupyter Notebook script can be run to nicely format word document interview transcripts (for example exported from REV) to be imported into NViVo. 

https://docs.anaconda.com/ae-notebooks/4.3.1/user-guide/basic-tasks/apps/jupyter/

# Export from REV Settings
Output Format: In-line
File Type: *.docx
Export Options: Include speaker names

# Word Document Format
The word document should follow the following formatting:

speaker title
speaker quote
speaker title 2
speaker 2 quote

There should be now extra enters in the document. See sample.

# Sample
There is a sample dialouge (from Midnight Gospel Episode 8 on Netflix). You should be able to run the jupyter notebook no problem on this sample. 

# Verify your Work
Check word counts between the original and the formatted to make sure everything is accounted for. If you are using rev files, this script automatically removes the 'part X of X' from the file. So be sure to account for the loss of these words. 

# How to change jupyter notebook start up location
1. Open cmd (or Anaconda Prompt) and run: jupyter notebook --generate-config
2. This writes a file to C:\Users\(username)\.jupyter\jupyter_notebook_config.py.
3. Browse to the file location and open it in an Editor
4. Search for the following line in the file: #c.NotebookApp.notebook_dir = ''
5. Replace by c.NotebookApp.notebook_dir = '/the/path/to/home/folder/'

I use 'C:/'

Make sure you use forward slashes in your path and use /home/user/ instead of ~/ for your home directory, backslashes could be used if placed in double quotes even if folder name contains spaces as such : "D:\yourUserName\Any Folder\More Folders\"

6. Remove the # at the beginning of the line to allow the line to execute when opening