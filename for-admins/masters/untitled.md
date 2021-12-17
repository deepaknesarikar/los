---
description: >-
  Schemas are very important for validating the master while uploading via excel
  or while adding / editing any record.
---

# Schemas

| **Sch**ema      | Type                                                                                                                                              | Description                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
| --------------- | ------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| _Column Name_   | Free Text                                                                                                                                         | The column name will be required to be the column header in the excel                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| _Data Type_     | <p>Dropdown with values</p><ul><li>Numeric</li><li>Boolean</li><li>Alphanumeric</li><li><p>Pipe Separated</p><p>Semicolon Seperated</p></li></ul> | <p>All the master columns will have pre-defined data types which will be used to check and validate any wrong entry in the master. The data types are as below</p><ul><li>Numeric: Will only allow numbers in the column. They may contain decimals as well</li><li>Boolean: Will only allow value from false / FALSE / true / TRUE.  Anything other than these values won't be allowed</li><li>Alphanumeric: Will allow characters from a-z and 0-9. Special characters and symbols won't be allowed</li><li>Pipe Separated: You can add multiple values in the same column using this data type. </li></ul> |
| _Mandatory_     | Boolean                                                                                                                                           | Marking the column as mandatory will check for each cell in the master of that column for not null. I.e. mandatory column cannot have any cell as blank                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| _Default Value_ | Free Text                                                                                                                                         | <p>Default value will be used to handle the schema changes after the master is uploaded. Consider below scenario</p><p>First time the master was uploaded, it had 3 columns. Later the 4th column was added with mandatory check. Then the code will update the 4th column of master with the default value.  Next time when you upload, you can upload the correct values in the 4th column</p>                                                                                                                                                                                                              |