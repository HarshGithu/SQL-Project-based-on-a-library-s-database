# SQL-Project-based-on-a-library-s-database![68747470733a2f2f692e696d6775722e636f6d2f63304e566272792e706e67](https://user-images.githubusercontent.com/108324235/177376639-1b38c968-a4dd-4d1e-aea0-50464db1beec.png)
Normalization

CARD (Number, Fines, Status)

CUSTOMER (ID, Name, Address, Phone_number, Card_number [References CARD(Number)], Password, User_name, Date_sign_up)

EMPLOYEE (ID, Name, Address, Phone_number, Card_number [References CARD(Number)], Password, User_name, Paycheck, Branch_name [References BRANCH(Name)])

BRANCH (Name, Address [References LOCATION(Address)], Phone_number)
LOCATION (Address)

RENT (Card_ID [References CARD(Number)], Item_ID [References BOOK or VIDEO(ID)], Date, Return_date)

BOOK (ISBN, ID, State, Avalability, Deby_cost, Lost_cost, Address [References LOCATION(Address)])

VIDEO (Title, Year, ID, State, Avalability, Deby_cost, Lost_cost, Address [References LOCATION(Address)])
