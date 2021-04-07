---
permalink: /chase-hospitals/features/
title: "Features"
author_profile: false
sidebar:
  nav: "chase-hospitals"
---

I have made a short video explaining all the features of this project. You can view it [here](https://youtu.be/Z7PExj_v-ZU) (and make sure to like the video :sparkling_heart:)       
<iframe width="560" height="315" src="https://www.youtube.com/embed/Z7PExj_v-ZU" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

Every window/page has voice feedback so its literally someone talking and explaining things as you click them.

# Connecting to Database

As soon as you enter the main window, you are asked to fill your MySQL username and password. 
By-default your username is taken as root, however you can change it. 
	
![mysql-username](/assets/chase-hospitals/mysql-username.webp)

![mysql-password](/assets/chase-hospitals/mysql-password.webp)

# Main Window

There are 7 buttons on the left side, which provide all the basic things necessary for a Hospital. In the centre there is the main logo.

![main-window](/assets/chase-hospitals/main-window.webp)

# Registration

As you click on the button, a computerised voice would announce all the details that needs to filled.

![registration](/assets/chase-hospitals/registration.webp)

After filling of details, you would be given your PID. This is required to access other cool things.

![after-registration](/assets/chase-hospitals/after-registration.webp)

# Appointment

After registering yourself, patients can make an appointment with existing Doctors. They have to identify themselves by filling their PID. They can also select a date from the pop-up calendar. After submiting, general instruction regarding SOP is shown.

![after-appointment](/assets/chase-hospitals/after-appointment.webp)

# Patient Details

When you click on the patient details button, a drop down menu listing possible fields and a empty text box would be visible. All you need to do is to select a field and enter your value to search.
You can search a patient using any of the field. However if there are multiple entries available in the database (say 'Male' as gender) then voice feedback would notify you no. of duplicate entries found and ask you again to select another field and search again. 
This time your previous field as well as your new field both would be used to find the patient. However, if duplicate entries are found again then this would continue till all 4 fields are used. If the patient is not found till then, all previous fields would be cleared and you would be returned to the main window.

![search-patients](/assets/chase-hospitals/search-patient.webp)

The best way to find your patient is using your PID as it is unique and you can easily find your patient. After successfully finding your Patient, a new page would be visible. All the details of the patient along with their appointment would be visible. A randomly selected profile pics would also be visible.

![patient-details](/assets/chase-hospitals/patient-details.webp)

# Modify Details

Say you want to change any details about your patient. You can do it easily by clicking on the modify details button. You would be asked to fill your PID. After successfully verifying yourself, all your details would be shown. 
Underneath it a drop down menu listing all the fields would be given. You can select any of the field and then fill the new information in the text box. When you click on submit, your details would be updated and you would be notified and return to main window.

![modify-details](/assets/chase-hospitals/modify-details.webp)

# Doctor Details

It is a static window which showcases all the details of existing doctors.

![doctor-details](/assets/chase-hospitals/doctor-details.webp)

# Services Offered

This is also a static window to display default data. It showcases no. of image carousel where you can see different (free - use) image of the hospital (laboratories, operation theatre etc.)

![services-main-window](/assets/chase-hospitals/rooms.webp)

![image-carousel](/assets/chase-hospitals/image-carousel.webp)

# About Us

There is also an About Us window where little information regarding the project, developers and our Teacher is given.

![about](/assets/chase-hospitals/about.webp)