# RunTrackingAPIs
Technoloy:
python 3.5
sqllite


Admin Site URL:
baseurl/admin
API Root URL:
baseurl/api


LoginAPI: /api/token
Verb: Post
RequestBody:{ "username":"admin", "password":"password123" } 

CreatSession /api/sessions/
verb: POST
RequestObject: {"duration":"","miles":""}
GetSessions:/api/sessions/
Verb:Get
PreRequisite: Valid Auth token i.e Authorization: token 81a06838b4952cf192f5227150420ada18f712b1

GetSessionById: /api/sessions/{id}/    i.e api/sessions/3/  
Verb:Get
PreRequisite: Valid Auth token 


GetSpeedById:/api/sessions/{id}/Speed/
Verb:Get
PreRequisite: Valid Auth token 

GetDistanceById: /api/sessions/{id}/Distance/
Verb:Get
PreRequisite: Valid Auth token 
GetTotalSpeed:/api/sessions/TotalSpeed/
Verb:Get
PreRequisite: Valid Auth token 

GetTotalDistance:/api/sessions/TotalDistance/
Verb:Get
PreRequisite: Valid Auth token

GetUsers: /api/users/
Verb:Get

GetUserByName: /api/users/{username}/  i.e api/users/admin/
Verb:Get

CreateUser:
