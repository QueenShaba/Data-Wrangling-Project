# Data-Wrangling-Project
Wrangling the WeRateDogs Twitter data to create interesting and trustworthy analyses, and visualizations.
Reporting: wragle_report In the wrangle project three steps; Gather, Assess, and Clean! were used to achieve success in analysing the ‘WeRateDogs’ 
datasets.

Gather Three datasets were gathered from different sources, they include; twitter_archive_enhanced.csv given by Udacity, this dataset was read into the
python notebook. Secondly, the tweet_json.txt was also collected from Udacity’s archive because the author was unable to asses twitter. The tweet_json.txt 
was read into the python notebook. Finally, the third dataset image_prediction.tsv hosted on Udacity's servers, was downloaded programmatically using the 
Requests library.

Assess For assessment, the study was required to generate visual and programatically assessed issues to correct, although a number of problems could be 
since it was enough to identify eight quality issues and two tidiness issues to solve. Visual assessment involved exporting the datasets to external 
software like google sheets to view row by row and column by column, resulting in identifying some errors in the datasets. For programmatic assessment, 
code was used to ask specific questions for instance datatypes of the columns to see if there were inconsistencies to be addressed, and they were! The
quality issues generated are categories below by datasets and whether or not they were obtained visually or programmatically, they include; From 
df_TwitterArchive Incomplete and irrelevant columns with NaN inputs, examples are 'in_reply_to_status_id', 'in_reply_to_user_id', 'retweeted_status_id'
and so on should be dropped. (Visually assessed) Invaid data type for timestamp, expecting datetime not string. (Programatically assessed) Presence of 
invalid dog names such as 'none', 'a', 'the' and 'an'. (Programatically assessed) From df_ImagePredict P1, P2, and P3 columns have rows with names 
starting in lowercase for some and uppercase for others. (Visually assessed) P1, P2, and P3 columns have rows with names separeted by an underscore 
insted of space. (Visually assessed) Drop img_num column as it is irrevant to the study. (Visually assessed) Rows with missing photos for tweet_id and 
all other columns i.e. 2354 rows instead of 2075 as in df_TwitterArchive. (Programatically assessed) From df_TweetApi Rows with missing entries i.e. 
2354 rows instead of 2356 as in df_TwitterArchive. (Programatically assessed) General Invalid data type for tweet_id, expecting string not integer. 
(Programatically assessed) The tidiness issues generated are listed below and they were obtained visually, they include; Separate doggo, floofer, pupper 
and puppo columns which should be combined as one column in df_TwitterArchive. The df_TwitterArchive, df_ImagePredict, and df_TweetApi dataset should be 
combined to generate one dataset. Clean This was the most exciting part of the project, the quality and tidiness issues created were cleaned using the 
define, code and test steps. Each issue was defined or spelled out, the code for cleaning was generated and implemented and finally tests were carried out
to ensure the changes were made. Befor the steps above were carried out, a copy of the master merged data was made to preserve the original data.

Finally, the dataset was stored, insights generated and visuals created to complete the project.
