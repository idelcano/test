build:

python3 setup.py bdist_wheel

intall module:
sudo pip3 install git+http://github.com/idelcano/test.git#egg=testina

example of call:

import testina.dhis2api

api = testina.dhis2api.Dhis2Api("http://localhost:8080", "user", "pass")

print(api.get('/me'))
