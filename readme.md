# Patient Self Service Portal - Admin View

### Description

In this repository, our patient self-service portal becomes more fleshed out with the addition of tangible tables, dummy data, and adding/editing/updating/deleting features. Using our given source code as a base, we ensure that our data is connected to the app properly by adjusting table connections and endpoint parameters in `app.py`. To ensure that our information is displayed correctly, we focus mainly on `patient_all.html` and `patient_details.html`.

Specifically, from the source code, we have adapted three new fields for patients: Sex, Birthdate, and Zip Code, based on `gender`, `dob`, and `zip_code` fields from our original `patient_portal.patients` table. These fields are added uniformly across the patient master list, the individual patient info views, as well as where relevant when adding and updating patient information.

### Components

The four components found in this repository are:

- **`app.py` (Python Script)**
  - Our Python script for launching and maintaining our app.

- **`templates` (Folder)**
  - This folder houses our HTML files.

- **`static` (Folder)**
  - This folder houses our CSS files.

- **`images` (Folder)**
  - This folder houses image files picturing the following:
    - The `/patients` list page with dummy data and the three newly added fields
    - The `/view` page of a single patient with the three newly added fields
    - The modal window for editing a patient's details with the three newly added fields available for editing and updating
    - The modal window for adding a new patient with the three newly added fields available for editing and updating
