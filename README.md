```
$ nosetest -v
Test the login function when bad creds are passed. ... ok
Test the login function when an error happens. ... ok
Test the login function when things go right. ... ok

----------------------------------------------------------------------
Ran 3 tests in 0.004s

OK

$ pylint -r n project1/
No config file found, using default configuration
************* Module project1
C:  1, 0: Missing module docstring (missing-docstring)
************* Module project1.authentication
C:  4, 0: Missing function docstring (missing-docstring)
W: 13,11: Catching too general exception Exception (broad-except)
W: 13,22: Unused variable 'exc' (unused-variable)

$ nosetests --with-coverage --cover-package=project1
...
Name                      Stmts   Miss  Cover   Missing
-------------------------------------------------------
project1                      0      0   100%
project1.authentication      12      0   100%
-------------------------------------------------------
TOTAL                        12      0   100%
----------------------------------------------------------------------
Ran 3 tests in 0.010s

OK
```
