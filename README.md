# !! NOT IMPLEMENTED YET - DON'T USE !!

## Library Sim800L Module for Cypress PSoC Family
The Purpose of This library is to use the module in the most easy way and transparent.  
Website: [Sim800L library](https://github.com/VittorioEsposito/Sim800L-revised)



## Methods and functions

Name|Return|Notes
:-------|:-------:|:-----------------------------------------------:|
begin()|None|Initialize the library
begin(number)|None|Initialize the library with user's baud rate
reset()|None|Reset the module, and wait to Sms Ready.
setSleepMode(bool)|bool|enable or disable sleep mode *
getSleepMode()|bool|return sleep mode status *
setFunctionalityMode(number)|bool|set functionality mode *
getFunctionalityMode()|bool|return functionality mode status *
setPIN(String)|bool|enable user to set a pin code *
getProductInfo()|String|return product identification information
getOperatorsList()|String|return the list of operators
getOperator()|String|return the currently selected operator
calculateLocation()|bool|calculate gsm position *
getLocationCode()|String|return the location code
getLongitude()|String|return longitude
getLatitude()|String|return latitude
sendSms(number,text)|bool|both parameters must be Strings. *
readSms(index)|String|index is the position of the sms in the prefered memory storage
getNumberSms(index)|String|returns the number of the sms.
delAllSms()|bool|Delete all sms *
signalQuality()|String|return info about signal quality
answerCall()|bool| *
callNumber(number)|None|
hangoffCall()|bool| *
getCallStatus()|uint8_t|Return the call status, 0=ready,2=Unknown(),3=Ringing,4=Call in progress
setPhoneFunctionality()|None|Set at to full functionality 
activateBearerProfile()|None|
deactivateBearerProfile()|None|
RTCtime(int *day,int *month, int *year,int *hour,int *minute, int *second)|None| Parameters must be reference ex: &day
dateNet()|String|Return date time GSM
updateRtc(utc)|bool|Return if the rtc was update with date time GSM. 
____________________________________________________________________________________
