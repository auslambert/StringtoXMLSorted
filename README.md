# StringtoXMLSorted v4
More features added.

Creates an Xml file with data sets that are editable with a standard XML editor such as Notepad for XML in a location of your choice,
Either the /NVRAM root folder or the /NVRAM/<ProgramID> folder. You could probably specify a fully qualified file path to anywhere 
but I haven't tested that.
  
Each data record contains a elements in the format:
<recordX>
  <Field1>
  </Field1>
  <Field2>
  </Field2>
</RecordX>
* Up to five fields are accomodated.
* Records can be sorted by field1 ascending/decending/not sorted.
* If all fields in a records are empty the records will be dropped (deleted).
  
In the SIMPL folder is an example program that contains example SIMP code plus the required S+ modules for one through five fields.
The example modules define 25 data pairs but the S# doesn't care, only writing those elements that have data in at least one field.
You can customize the max number of records passed to SIMPLsharp by altering the line in the S+ file:
#DEFINE_CONSTANT ASIZE 25 and recompiling.

The example code has been tested on a 4 series processor.
  
I dropped the other utilites found in the V1 example.
  
Enjoy!
