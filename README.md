# User Enumeration
User Enumeration on Umanni RH

==

# Description

A user enumeration vulnerability flaw was found in Umanni RH. This issue occurs during password recovery, where a difference in messages could allow an attacker to determine if the user is valid or not, enabling a brute force attack with valid users.

==

# Exploitation

To exploit this vulnerability, it is necessary to request a password recovery, when adding a valid contact email the message: "You will receive and email with instructions about how to reset your password in a few minutes." is displayed and when an invalid email: "Email not found".

==

# PoC

== Invalid User ==

![4_](https://user-images.githubusercontent.com/49153346/87189829-be95f300-c2c7-11ea-8f1f-482d2bc15f58.jpg)

== Valid User (Redirect) ==

![5_](https://user-images.githubusercontent.com/49153346/87189427-00726980-c2c7-11ea-94f1-c4967eb4ac3f.JPG)

== Valid User ==

![6_](https://user-images.githubusercontent.com/49153346/87189549-3dd6f700-c2c7-11ea-9ce2-a26fdc1e8a81.jpg)

== Brute Force - Invalid User ==

![9__](https://user-images.githubusercontent.com/49153346/87189889-da00fe00-c2c7-11ea-9530-559fbee179be.jpg)

== Brute Force - Valid User (Redirect) ==

![10__](https://user-images.githubusercontent.com/49153346/87190303-9ce93b80-c2c8-11ea-8bdd-0c967d0d5205.jpg)

== Brute Force - Valid User ==

![11__](https://user-images.githubusercontent.com/49153346/87189929-ec7b3780-c2c7-11ea-900a-69304e6e89c1.jpg)
