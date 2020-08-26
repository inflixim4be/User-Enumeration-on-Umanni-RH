<h2 align="center">
  CVE-2020-24008 
  <br/>
  User Enumeration on Umanni RH
</h2>

<p align="center">
  <img src="https://user-images.githubusercontent.com/49153346/88341987-f021ac00-cd14-11ea-836b-0fba611d7540.png" width="350" />
</p>

<hr>

### Description

A user enumeration vulnerability flaw was found in Umanni RH. This issue occurs during password recovery, where a difference in messages could allow an attacker to determine if the user is valid or not, enabling a brute force attack with valid users.


### Exploitation

To exploit this vulnerability, it is necessary to request a password recovery, when adding a valid contact email the message: "You will receive and email with instructions about how to reset your password in a few minutes." is displayed and when an invalid email: "Email not found".


### PoC

* Invalid User 

<img src="https://user-images.githubusercontent.com/49153346/87189829-be95f300-c2c7-11ea-8f1f-482d2bc15f58.jpg"/>

<br />

* Valid User (Redirect) 

<img src="https://user-images.githubusercontent.com/49153346/87189427-00726980-c2c7-11ea-94f1-c4967eb4ac3f.JPG"/>

<br />

* Valid User 

<img src="https://user-images.githubusercontent.com/49153346/87189549-3dd6f700-c2c7-11ea-9ce2-a26fdc1e8a81.jpg"/>

<br />

* Brute Force - Invalid User 

<img src="https://user-images.githubusercontent.com/49153346/87189889-da00fe00-c2c7-11ea-9530-559fbee179be.jpg"/>

<br />

* Brute Force - Valid User (Redirect) 

<img src="https://user-images.githubusercontent.com/49153346/87190303-9ce93b80-c2c8-11ea-8bdd-0c967d0d5205.jpg"/>

<br />

* Brute Force - Valid User 

<img src="https://user-images.githubusercontent.com/49153346/87189929-ec7b3780-c2c7-11ea-900a-69304e6e89c1.jpg"/>
