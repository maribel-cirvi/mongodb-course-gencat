### Mongosh Path
C:\Cursos\MongoDB\Executables\mongosh\bin

### Mongosh Executes an external javascript file
mongosh "127.0.0.1/school" scripts\CreateSchoolSchema.js
mongosh "127.0.0.1/school" scripts\GetStudents.js

mongosh "mongodb+srv://cluster0.8mwtier.mongodb.net/school" --apiVersion 1 --username mongobel
mongosh "mongodb+srv://cluster0.8mwtier.mongodb.net/school" --apiVersion 1 --username mongobel scripts\CreateSchoolSchema.js

### Execute Postman files via Newman
newman run NttData-student-gencat.postman_collection.json -e NttData-Student-PRO.postman_environment.json

### Execute Newman's Report
npm install -g newman-reporter-htmlextra
newman run NttData-student-gencat.postman_collection.json -e NttData-Student-PRO.postman_environment.json -r htmlextra 
- in folder newman we will get an html report file
