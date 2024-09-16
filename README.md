# Code_Breakers
from request import session

Session = session()

payload = {
    "username": Test,
    "password": "Dragoo",
    "testtest": "1",
    "browser": "Chrome_57"
    }

result = Session.post("https://forms.office.com/Pages/DesignPageV2.aspx?origin=Marketing&fromar=1&subpage=creationv2",data=payload).content.decode() #Session.get for get request

print(result) 
