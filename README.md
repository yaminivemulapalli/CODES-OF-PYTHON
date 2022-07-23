# CODES-OF-PYTHON
#default email id by concatenating the users first and last name:
class person:
    domain_name="@gmail.com"
    def __init__(self,fname,lname,age):
        self.fname=fname
        self.lname=lname
        self.age=age
    def full_name(self):
        return str(self.fname)+str(self.lname)
    def __str__(self):
        print("Email i'd:",str(self.fname)+str(self.lname)+person.domain_name)
fname=str(input("enetr the first name"))
lname=str(input("enetr the last name"))
age=int(input("enetr the age"))
obj=person(fname,lname,age)
obj.__str__()
