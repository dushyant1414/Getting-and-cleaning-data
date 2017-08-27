Codebook

1.  Required columns are identified using grep()  function

2.  Subject, activity and feature data for only the required columns is
    combined into test and train from the testing and training datasets
    respectively

3.  These two are then combined into allData using rbind

4.  allData columns are labelled for the imported feature data

5.  allData is then melted (using reshape2 package) into "long" format,
    and then dcast into wide format while calculating the mean of each
    feature data by subject and activity

6.  This is exported into tidy.txt
