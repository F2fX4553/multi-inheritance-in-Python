# multi-inheritance-in-Python
class human:
    def __init__(self,name,age):
        self.name = name
        self.age = age

class ductor:

    def __init__(self,stayle):
        self.stayle = stayle

class studnt(human , ductor):

    def __init__(self,name,age,stayle):
        human.__init__(self,name,age)
        ductor.__init__(self,stayle)


    def printdata(self):
        print(self.name,self.age,self.stayle)


pos = studnt('oussama',25,'rap')
pos.printdata()
