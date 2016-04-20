This effort at REACHnet builds on the [Cajun Codefest 4.0](http://www.cajuncodefest.org/index.php/event-info/competition-rules). The codefest provided a FHIR api of 300 de-identified patients, to facilitate development of SMART-on-FHIR apps for Diabetes.



## How to sign Data Use Agreement?

## How to access FHIR endpoint?

Endpoint: [https://demo.hioh.org/srv-dstu2-0.3/api](https://demo.hioh.org/srv-dstu2-0.3/api)

Number of patients: 300

###CODEATHON INSTRUCTION MATERIAL

**Contents** 

1. Prerequisite 
2. REST client for Firefox 
3. Adding token to the header 
4. API’s 
5. Invalid token 
6. Get All Patients 
7. Get Patient details 
8. Get Labs for a particular patient 
9. Get Conditions for a particular patient 
10. Sample SMART App

**1. Prerequisite**

In order to call the FHIR API’s, you need a REST client on your PC.
REST client add on is available for Firefox browser.
POSTMAN REST client is available for Chrome browser.

We recommend using Firefox REST client and this document explains the usage for the same.

Firefox browser can be downloaded at:
https://www.mozilla.org/en-US/firefox/new/?utm\_source=google&utm\_medium=paidsearch&utm\_campaign=sem2015Q4&utm\_term=nonbrand&utm\_content={meta%20data}

Chrome browser can be downloaded at:
https://www.google.co.in/chrome/browser/desktop/

**2. REST client for Firefox**

Make sure that REST client add on in installed on the Firefox browser.
To configure it for your browser, please follow the below steps:

1. To install it from internet please navigate to:
https://addons.mozilla.org/en-US/firefox/addon/restclient/
2. Click on “Add to Firefox”
3. Once the installation is complete, restart the Firefox browser
4. Click on the REST client logo in the toolbar as shown below

**3. Adding token to the header**

1. Click on the “Headers” present in the top bar and select “Custom Headers”
2. You need to add the token as a header field
Name: Authorization
Value: Bearer {tokenstring}
3. Click on Okay

**4. API’s**

There are four API’s available as mentioned below:

1. API to get the list of all the patients:
https://demo.hioh.org/srv-dstu2-0.3/api/Patient
2. API to get the patient details:
https://demo.hioh.org/srv-dstu2-0.3/api/Patient/{patient_id}
3. API to get Labs for a particular patient
https://demo.hioh.org/srv-dstu2-0.3/api/Observation?subject={patient_id}
4. API to get Conditions for a particular patient
https://demo.hioh.org/srv-dstu2-0.3/api/Condition?patient={patient_id}

**5. Invalid token**

1. Select Method as “GET”
2. Enter URL as https://demo.hioh.org/srv-dstu2-0.3/api/Patient
3. Click on “SEND”
4. Once the response is received, click on Response Body (RAW)
5. If the entered token is invalid/ incorrect, “Authentication Failure” message will be display.

**6. Get All Patients**

1. Select Method as “GET”
2. Enter URL as https://demo.hioh.org/srv-dstu2-0.3/api/Patient
3. Click on “SEND”
4. Once the response is received, click on Response Body (RAW)

**7. Get Patient details**

1. Select Method as “GET”
2. Enter URL as https://demo.hioh.org/srv-dstu2-0.3/api/Patient/{Patient_id}
   Where, {patient_id} = ID for one of the patients
3. Click on “SEND”
4. Once the response is received, click on Response Body (RAW)

**8. Get Labs for a particular patient**

1. Select Method as “GET”
2. Enter URL as https://demo.hioh.org/srv-dstu2-0.3/api/Observation?subject={patient_id}  
3. Click on “SEND”
4. Once the response is received, click on Response Body (RAW)

**9.	Get Conditions for a particular patient**

1.	Select Method as “GET”
2.	Enter URL as https://demo.hioh.org/srv-dstu2-0.3/api/Condition?patient={patient_id} 
     Where, {patient_id} = ID for one of the patients
3.	Click on “SEND”
4.	Once the response is received, click on Response Body (RAW)

**10. Sample smart apps**

[Diabetes app](https://demo.hioh.org/applib-dstu21-0.3/diabetes-monograph/launch.html?iss=https://demo.hioh.org/srv-dstu2-0.3/api)
This app was ported from the SMART-App gallery.

## How to import data in PCORNet CDM format into i2b2?

## Contact and mailing list

##[Cajun Codefest 4.0](http://www.cajuncodefest.org/index.php/event-info/competition-rules)
--summary of the codefest

