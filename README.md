# User-defined-Exception
class ToYoungExecption(Exception):
    def __init__(self,arg):
        self.msg=arg

class ToOldException(Exception):
    def __init__(self,arg):
        self.msg=arg

age=int(input('Enter your age:='))
if age<18:
    raise ToYoungExecption("please wait some time you will get better match")

elif age>60:
    raise ToOldException('You are too old to marriage')
else:
    print('Thank you for registation, You will get your match soon')
