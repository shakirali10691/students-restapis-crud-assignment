# students-restapis-crud-assignment
Create an application with Restful APIs using Vertx or Springboot for CRUD operation to a TABLE of STUDENT(s) in a School in a PostgresDB

Create an application with Restful APIs using Vertx or
Springboot for CRUD operation to a TABLE of STUDENT(s)
in a School in a PostgresDB
The Table should have the following column.
ID NAME DATE OF BIRTH JOINING DATE CLASS
You should be able to
• ADD a STUDENT to the table.
• GET details of STUDENT(s) by ID or NAME or CLASS
• UPDATE details for the STUDENT(s)
Please push the project repo to github (ensure public acess)and provide back the URL and
have it setup to run locally on your device.

***student CRUD operations of restapis endpoints using Spring Boot with PostgresSQL are:---

(1.) create student rest api
url:-- http://localhost:8080/api/v1/create-students

request:-- {
   "name":"Shakir Ali",
   "date_of_birth":"10/06/1991",
   "joining_date":"19/01/2015",
   "std_class":"IT Software Development"
}

response:-- {
    "id": 10,
    "name": "Shakir Ali",
    "date_of_birth": "10/06/1991",
    "joining_date": "19/01/2015",
    "std_class": "IT Software Development"
}

(2.) get student by id rest api
url:-- http://localhost:8080/api/v1/students-find/4

request:-- get APIs fetching through url

response:--
{
    "id": 4,
    "name": "Zoya Khan",
    "date_of_birth": "10/06/1991",
    "joining_date": "22/11/2023",
    "std_class": "MCA"
}

(3.) update/edit student rest api
url:-- http://localhost:8080/api/v1/students-edit/1

request:-- {
   "name":"Sana Ali Khan",
   "date_of_birth":"17/11/1993",
   "joining_date":"20/12/2021",
   "std_class":"D.Pharma"
}

response:-- {
    "id": 1,
    "name": "Sana Ali Khan",
    "date_of_birth": "17/11/1993",
    "joining_date": "20/12/2021",
    "std_class": "D.Pharma"
}

(4.) get or fetch all student list records
url:-- http://localhost:8080/api/v1/students-list

request:-- get APIs fetching through url

response:-- [
    {
        "id": 2,
        "name": "Feeda Hussain",
        "date_of_birth": "26/04/2025",
        "joining_date": "15/12/2018",
        "std_class": "M.Tech"
    },
    {
        "id": 3,
        "name": "Sameer Khan",
        "date_of_birth": "10/06/0191",
        "joining_date": "20/01/2015",
        "std_class": "B.Tech"
    },
    {
        "id": 4,
        "name": "Zoya Khan",
        "date_of_birth": "10/06/1991",
        "joining_date": "22/11/2023",
        "std_class": "MCA"
    },
    {
        "id": 1,
        "name": "Sana Ali Khan",
        "date_of_birth": "17/11/1993",
        "joining_date": "20/12/2021",
        "std_class": "D.Pharma"
    },
    {
        "id": 5,
        "name": "Zoya Khan dfgdfsg",
        "date_of_birth": "31/12/1995",
        "joining_date": "22/11/2027",
        "std_class": "MBA"
    },
    {
        "id": 6,
        "name": "Sajida Ali Khan",
        "date_of_birth": "30/07/1994",
        "joining_date": "19/12/2025",
        "std_class": "NEET"
    },
    {
        "id": 7,
        "name": "Sajida Ali Khan sdfadf",
        "date_of_birth": "30/07/1994",
        "joining_date": "19/12/2025",
        "std_class": "NEET sdfasf"
    },
    {
        "id": 9,
        "name": "Sajida Ali Khan sdfadf new",
        "date_of_birth": "30/07/1994",
        "joining_date": "19/12/2025",
        "std_class": "NEET sdfasf bbb"
    },
    {
        "id": 10,
        "name": "Shakir Ali",
        "date_of_birth": "10/06/1991",
        "joining_date": "19/01/2015",
        "std_class": "IT Software Development"
    }
]

(5.) delete students rest api
url:-- http://localhost:8080/api/v1/students-delete/8

request:-- request:-- delete APIs through url

response:-- {
    "Student record deleted sucessfully.": true
}

