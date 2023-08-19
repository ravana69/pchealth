# pchealth

Check System Installation Date: 

systeminfo | find "Original Install Date"

================================================

Check Event Logs for Critical Events:

wevtutil qe System /f:text /c:1 /rd:true /q:"*[System[(EventID=41)]]"
