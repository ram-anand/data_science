# Resume parser utlity

#### It can multipage resumes in process word (.doc & .docx) and pdf (.pdf) files

### Web Instance:
- Resumes can be uploaded to local url home url: http://127.0.0.1:PORT_NUMBER
- On submit , it redirects to output page with parsed resume data in form of table output url: http://127.0.0.1:PORT_NUMBER/output
- It also generates two extract file of parsed tabular data (RESUME_DUMP.CSV, RESUME_DUMP.TXT)

#### Note: It can not process old word (.doc) file

### Local Instance
- Resumes are placed in the directory indicated by constant "RESUME_FOLDER"
- To enable local instance, uncomment local instance main method in below code (also disable the web instance main method at the same time)
- Run the jupyter notebook to run resume parser
- It also generates two extract file of parsed tabular data (RESUME_DUMP.CSV, RESUME_DUMP.TXT)

#### Note: It can process word (.doc & .docx) and pdf (.pdf) files. To process (.doc) file, it first converts them into (.docx) file.

### Library Dependency
- pdfminer - to read (.pdf) file
- docx2txt - to read (.docx) file
- spacy/nltk - for pattern matching and entity recognition
