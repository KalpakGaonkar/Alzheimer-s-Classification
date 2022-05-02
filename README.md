# Alzheimer's Classification

## This is a system consisting of a web application and an android application. The web application uploads the MRI scan of the patient to a machine learning model which classifies the stage and uploads both the stage and the scan to the database along with some more patient information. The android application displays the patient information and MRI scans on the device

## Repository Links

1. Web Application: https://github.com/KalpakGaonkar/AlzCareWebApp
2. Android Application: https://github.com/KalpakGaonkar/alzApp

## 1. Web Application
This is a web a application developed using JavaScript and meant to serve as a directory of patients under the care of a doctor

## 2. Android Application
App that aims to help people with Alzheimer's disease and their caregivers

## Product Requirements

Goal (Web Application): Allow doctor to successfully maintain a database of patients
Goal (Android App): Allow user to successfully log in and view their details

## Functional Requirements and User Stories

## 1. Web Application

|  | User Story | Requirement |Priority|Status|
|---|---|---|---|---|
|Login on Device|As an existing user I want to be able to login to my account|The system must allow users to login using their email and password|Must Have|Completed|
|Update profile|As an existing user I want to be able to update my profile|The system must allow users to update their profile|Must Have|Completed|
|Add, update and delete patients|I should be able to add new patients to the system|The system must be able to add new patients, update their information or delete patients|Must Have|Completed|
|Display patient details|My existing patients should be visible to me|The system must display any patients added to the database|Must Have|Completed|
|Choose an MRI scan|As the doctor I should be able to choose a patient's MRI scan from the device|The system must be able to choose an MRI scan from the uesr's device|Must Have|Completed|
|Display MRI scan classification|As the doctor I should be able to view the classification of Alzheimer's and the upload button after choosing the image|The system must display the classification of MRI scan along with the **Upload** button after the doctor chooses the image|Must Have|Completed|
|Upload MRI scan|As the doctor I should be able to upload a patient's MRI scan|The system must be able to upload an MRI scan by pressing the **Upload** button|Must Have|Completed|

## 2. Android Application

|  | User Story | Requirement |Priority|Status|
|---|---|---|---|---|
|Create a new account|As a new user I want to be able to create an account|The system must allow user to create a new account using details like their name, email address and a password|Must Have|Completed|
|Login on Device|As an existing user I want to be able to login to my account|The system must allow users to login using their email and password|Must Have|Completed|
|Login as a patient or caregiver|As a user I want to be able to login as aa patient or a caregiver|The system must allow the user to login either as a patient or a caregiver|Must Have|Completed|
|Connect caregiver and patient|As a caretaker I want to enter my patient's name and be able to connect to their device|The system must be able to connect caregiver to the patient through unique keys in the database|Must Have|Completed|
|Display Patient Details|As an existing user I want to be able to see patient details on my phone|The system must fetch data from the database and display it on the device|Must Have|Completed|
|Display patient location|As a caregiver I want to see my patient's location|The system must be able to fetch location data from patient's device and display it on the caregiver's device|Must Have|Not Completed|
|Set Geofence|As a caregiver I want to set a geofence around my patient's location|The system must be able to fetch location data and set geofence around that location|Must Have|Not Completed|
|Send Geofence alert|As a caregiver I want to recieve an alert when my patient crosses the geofence boundary|The system must send out a notification alert when the patient's device crosses the geofence boundary set by the caregiver|Must Have|Not Completed|

---

## Use Case Diagrams

## 1. Doctor Module
Primary Actor: Doctor

<img src="https://github.com/KalpakGaonkar/Alzheimer-s-Classification/blob/main/Screenshots/doctor_use_case.png" width = 500 height = auto/>

## 2. Patient Module
Primary Actor: Patient

<img src="https://github.com/KalpakGaonkar/Alzheimer-s-Classification/blob/main/Screenshots/patient_use_case.png" width = 500 height = auto/>

## 3. Caregiver Module
Primary Actor: Caregiver

<img src="https://github.com/KalpakGaonkar/Alzheimer-s-Classification/blob/main/Screenshots/Caregiver_Use_case.png" width = 500 height = auto/>

---

## Architecture/ Flow Chart

<img src="https://github.com/KalpakGaonkar/Alzheimer-s-Classification/blob/main/Screenshots/Architecture%20.png" width = 1000 height = auto/>

---

## Activity Diagrams/ Flow of the modules

## 1. Doctor Module
<img src="https://github.com/KalpakGaonkar/Alzheimer-s-Classification/blob/main/Screenshots/activitydiagram_doctor.png" width = 500 height = auto/>

## 2. Patient Module
<img src="https://github.com/KalpakGaonkar/Alzheimer-s-Classification/blob/main/Screenshots/activitydiagram_patient.png" width=500 height=auto/>

## 3. Caretaker Module
<img src="https://github.com/KalpakGaonkar/Alzheimer-s-Classification/blob/main/Screenshots/activitydiagram_caretaker.png" width=500 height=auto/>

---

## Screenshots for the Web Application

## The dashboard

The dashboard is the first page that opens up after the doctor completes the log in process

<img src="https://github.com/KalpakGaonkar/patient-management-system/blob/main/Screenshots/Screen%20Shot%202022-04-22%20at%209.59.53%20AM.png" width = 1000 height = auto/>

## List of Patients

This page is visible after the doctor clicks on **My Patients** button from the navigation bar

There are two sections to this page:

- The first section is on the left side is the form for adding new patients to the list
- The second section is on the right side which displays the list of patients

![alt text](https://github.com/KalpakGaonkar/patient-management-system/blob/main/Screenshots/Screen%20Shot%202022-04-22%20at%2010.00.19%20AM.png)

## Patient Details

This page is visible after the doctor clicks on the patient's name on the **List of Patients** page

![alt text](https://github.com/KalpakGaonkar/patient-management-system/blob/main/Screenshots/Screen%20Shot%202022-04-22%20at%2010.00.37%20AM.png)

## Upload MRI scan

Clicking the upload button on a patient from the list on the **List of Patients** page prompts the doctor to upload an MRI scan image

The image is then passed to the machine learning model which displays the output of the MRI scan below the upload button (shown in the screenshot below)

After the output of the MRI scan is displayed, the doctor can click the Upload Button to upload the image and its classification to the database (Upload button not displayed until the classification of the MRI image is done by the machine learning model to prevent any errors)

![alt text](https://github.com/KalpakGaonkar/AlzCareWebApp/blob/main/Screenshots/Screen%20Shot%202022-04-22%20at%2010.00.49%20AM.png)

---

## Screenshots for Android Application

## Main page and sign in page

This is the main page that opens when you click on the application on your phone

After choosing sign in with email it takes you to the sign in page

<img src="https://github.com/KalpakGaonkar/alzApp/blob/main/Screenshots/Home_page_and_signin_page.png" width = 600 height = auto/>

## Option to choose patient or caregiver and Login page

After signing in, the application lets you choose to be either a patient or a caregiver and opens a log in page

<img src="https://github.com/KalpakGaonkar/alzApp/blob/main/Screenshots/patient_caregiver_option_and_login_page.png" width = 600 height = auto/>

## Patient and Caregiver Home Page

On the left is the patient home page which has features like create and remove reminder and the option of signing out

On the right is the caregiver home page which has features such as Adding a Patient, Viewing patient details, View geofences (Not Completed Yet) and the option of signing out

<img src="https://github.com/KalpakGaonkar/alzApp/blob/main/Screenshots/patient_and_caregiver_home_page.png" width = 600 height = auto/>

## List of Patients

This page displays the list of patient which is linked. A patient can be added using the "+" sign on the bottom right corner

<img src="https://github.com/KalpakGaonkar/alzApp/blob/main/Screenshots/list_of_patients.png" width = 300 height = auto/>

## Patient Details

This page displays the added patient's details which include updates from the doctor, the current stage of Alzheimer's and the MRI scan

<img src="https://github.com/KalpakGaonkar/alzApp/blob/main/Screenshots/patient_details.png" width = 300 height = auto/>
