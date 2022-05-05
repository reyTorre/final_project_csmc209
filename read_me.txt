###### --------------------------- All API End Points --------------------------------------

---- 1. Create User
https://azqg8rzrlk.execute-api.us-east-1.amazonaws.com/default/create_user_account?usr={value:string}&pas={value:string}&fir={value:string}&las={value:string}&rol={ADMIN/PATIENT}

---- 2. Log In
https://3rn2ddp1mc.execute-api.us-east-1.amazonaws.com/default/user_login?usr={value:string}&pas={value:string}

---- 3. Log OUT
https://p2n1exfrmh.execute-api.us-east-1.amazonaws.com/default/user-log-out?uid={value:string}

---- 4. Add Diary
https://t51171ce36.execute-api.us-east-1.amazonaws.com/default/add_diary?uid={value:string}&sys={value:number}&dia={value:number}

---- 5. Edit Diary
https://t5otup3pqg.execute-api.us-east-1.amazonaws.com/default/edit-diary-record?did=2&uid={value:string}&sys={value:number}&dia={value:number}

---- 6. Delete Diary
https://qkls0pwksl.execute-api.us-east-1.amazonaws.com/default/delete-diary?did={value:number}&uid={value:string}

--- 7. Get All Patients
https://u223pd1x4g.execute-api.us-east-1.amazonaws.com/default/get-all-patients

---8. Get All Diary Records
https://88ec03c96h.execute-api.us-east-1.amazonaws.com/default/get-diary-from-id?uid={value:string}

---9. Edit Records
https://ojsk04nu2e.execute-api.us-east-1.amazonaws.com/default/edit-user?uid={value:string}&usr={value:string}&fir={value:string}&las={value:string}&gen{value:string}&add{value:string}&mob={value:string}&bday={value:string}&ht={value:string}&wt={value:string}

Note:
{value:string} ---> data type is string
{value:number} ---> data type is number
{ADMIN/PATIENT} ---> Choices are either ADMIN/PATIENT


Architecture
REST API ----> Lamda Function (Python)
