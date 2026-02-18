---
name: metadata-genarator
description: Guide users through the process that can create an metadata file in JSON format.
---

# Create a metadata file

Step 1 Understand which JSON schema you need to build
Step 2 Get a sample of the data
Step 3 Ask questions to establish the unknown pieces of information
Step 4 Create the JSON schema



## Understanding which JSON schema you need to build
Get users to a point where you have generated a json format metadata file for them.


**Important** first ask the user to understand the source data format. Please ask them which of the following it is
1. SQL Database 
2. Raw Text File

Their answer to this question will determine which sample json schema you are defining. sample json schemas are called in the same format and saved in /json_formats/ and example format is the SQL Databases one will be called sql_databases.json and raw text files will be called raw_text_file.json.

**Important** don't do more then one step at once
## Getting a sample of the data

Next ask the user for a sample of their data, they can paste some rows of the data into chat. Do not move on until you have a sample of the data.

## Ask questions to establish the metadata you don't know

Based on the JSON file for every field you don't know from the sample ask the user questions to determine what these should be. Be clear about any assumptions you have made and ask the user if they are happy with these assumptions.

## Output the meta data file 

Once you have determined all the field save the metadata file as a .json file in a folder called metadata_json files in the users home directory. You may need to create the folder if it doesn't exist. If the user doesn't have a notebook open for you to use to do this in ask them to open a new workbook with compute running. You can then use this to generate and write the script which will generate the json file. Check the user is happy with you doing this, if they are not just give them the JSON file and tell them to copy and paste it into a new file.

## Playback to the user the file path 

Tell the user the filepath of the file you've created, with a link.
