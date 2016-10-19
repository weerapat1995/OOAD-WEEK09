# OOAD-WEEK09 Homework
##Class Diagram

###Class Diagram1_
Code

```
@startuml
Computer o-- Mainboard
Mainboard o-- Equipment
class Mainboard{
CPU 
RAM
Harddisk
}
class Equipment{
Mouse
Keyboard
Monitor
}
@enduml
```
Diagram

<img src="https://github.com/weerapat1995/OOAD-WEEK09/blob/master/HOMEWORK/Class1.png?raw=true">

###Class Diagram2_
Code
```
@startuml
Sale "*"--"1" Customer
Sale "*"--"1" Finance
Sale "1"--"*" Book
Sale "*"--"1" Manager
Finance "1"--"*" Order
Finance "1"--"1" Manager
Book "*"--"1" Order
Order "*"--"1" "A PRESS"
Order "*"--"1" Manager

class Sale{
+ S_ID
+ C_ID
- Number
- Price
+ Receip()
+ Dec_stock()
}
class Book{
+ B_ID
- B_Type
- B_Name
- Author
- Rate
- B_Value
- B_Price
- Number
+ Sale()
+ Search()
+ Order()
+ Stock()
}
class "A PRESS"{
+ A_ID
- A_Name
- A_address
- P_ID
+ Order()
+ Stcok()
}
class Finance{
+ F_ID
- F_Name
- F_Address
+ ReportSale()
+ ReportOrder()
+ Payment()
+ Receip()
}
class Customer{
+ C_ID
- C_Name
- C_Address
- Date_Begin
- Date_EXP
+ Resgit()
+ Sale()
}
class Manager{
- M_Name
- M_Address
+ ReportStock()
+ ReportSale()
+ ReportOder()
+ Stocl()
}
class Order{
+ P_ID
+ B_ID
+ B_Name
- P_Number
- Pay
+ Payment()
+ Inc_stock()
}
@enduml
```

Diagram

<img src="https://github.com/weerapat1995/OOAD-WEEK09/blob/master/HOMEWORK/Class2.png?raw=true">

###Class Diagram3_
Code
```
@startuml
Coffee <-- Member :Buy
Member <-- Empolyee :Service
Member --> Bill :Recive
Empolyee --> Bill :Create
Empolyee --> Purchase :Send
class Coffee{
- Name Coffee
- Cost
- ID
+ Sell()
+ Change Cost()
}
class Member{
- Name Member
- Sex
- ID
+ Call Name()
+ Call Genger()
+ Change Name()
}
class Empolyee{
- ID
- Name
- Genger
- Address
- Telephone
+ Change Name()
+ Call Genger()
}
class Bill{
- Bill_ID
- Date
- Name Product
- Cost Product
- Vat
- Amount Coffee
+ Add Product()
+ Add Amount Coffee()
}
class Purchase{
- Purchase_ID
- Date
- Name Product
- Cost
- Address Coffe Shop
+ Add Product()
+ Add Amount()
}
@enduml
```

Diagram

<img src="https://github.com/weerapat1995/OOAD-WEEK09/blob/master/HOMEWORK/Class3.png?raw=true">

###Class Diagram4_
Code
```
@startuml
Car -- Roadtrip
class Car{
+ ModelType
+ Doors
+ AutoMake
- Radio()
+ WimdshieldWiper()
+ ChangeDirection()
}
class Roadtrip{
+ Snacks
+ FuelLevel
- RadioStation
+ Route(start,end)
- Detour()
- PottyBreak()
}
@enduml
```

Diagram

<img src="https://github.com/weerapat1995/OOAD-WEEK09/blob/master/HOMEWORK/Class4.png?raw=true">

###Class Diagram5_
Code
```
@startuml
Car *-- Wheel
Driver -- Car
Person -- Car
@enduml
```


Diagram

<img src="https://github.com/weerapat1995/OOAD-WEEK09/blob/master/HOMEWORK/Class5.png?raw=true">



 
