as done in class and shown in the table, i can tell there is no price mentioned in row six (flagged) and the price is written with a comma in row 18 (1,250) making it a string which will cause invalid data since the program will treat this price as plain text while statistically analysing other prices (in floats). We need to either coerce this as an error or change the string to an float data type by stripping the comma. I have converted it to float since it might be important to the sample.  (correct)

moreoover, row 97 is also a duplicate of row 9 throughout all columns and therefore should be dropped. (exclude)

Lasty all columns are string based while prices should be numerica (float) and dates should be dateandtime -> (correct)
the codes for both are mentioned in the ipynb file