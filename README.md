# Internet-History

This is a Python script designed to extract data from Internet Explorer's index.dat files. It requires several external libraries (pytsk3, pyewf, pymsiecf, unicodecsv) that need to be installed beforehand.

To run the script, you need to open a terminal or command prompt and navigate to the folder where the script is saved. You can then type the following command:

python script_name.py evidence_file_path type_of_evidence [-d index_dat_directory_to_scan]

    evidence_file_path: The path to the image file or raw data file containing the index.dat files.
    type_of_evidence: The type of evidence file (either "raw" or "ewf").
    index_dat_directory_to_scan: The directory path where the index.dat files are located (optional; default is "/USERS").

Once the script finishes running, it will output a CSV file named "Internet_Indexdat_Summary_Report.csv" to the current working directory, containing the extracted data from the index.dat files. The CSV file will have the following columns:

    Index: The index of the record within the index.dat file.
    File Name: The name of the index.dat file.
    Record Name: The name of the record (if applicable).
    Record Type: The type of the record (if applicable).
    Primary Date: The primary date of the record (if applicable).
    Secondary Date: The secondary date of the record (if applicable).
    Last Checked Date: The last checked date of the record (if applicable).
    Location: The location of the record within the index.dat file.
    No. of Hits: The number of hits for the record (if applicable).
    Record Data: The data contained within the record (if applicable).
    Record Offset: The offset of the record within the index.dat file.
    File Path: The file path of the index.dat file within the image or raw data file.

If there are any errors during the script execution, they will be printed to the console.
