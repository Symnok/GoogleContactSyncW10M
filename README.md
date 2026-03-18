# GoogleContactsSync

**GoogleContactsSync** is an application for synchronizing **Google Contacts with Windows 10 Mobile (W10M) smartphones** using the **People APIl**.

The need for this application arose because built-in mail client does not sync contacts with Google anymore.

---

## Authentication

1.Enable Google People API:

Go to the Google Cloud Console. Create a new project (or select an existing one) https://console.cloud.google.com/projectcreate

Enable the "People API" for your project https://console.cloud.google.com/apis/api/people.googleapis.com/metrics?project=

See https://cloud.google.com/endpoints/docs/openapi/enable-api if you have a problem to enable API

Navigate to the API & Services Dashboard. Configure Consent Screen https://console.cloud.google.com/apis/credentials/consent?project= Define PeopleAPI scope as Contacts READ ONLY (second step of consent screen)

2.Set Up OAuth 2.0 Credentials:

In the API & Services Dashboard, go to "Credentials" https://console.cloud.google.com/apis/credentials?project= Create OAuth 2.0 Client ID credentials.

Download the JSON file with your credentials and save it under the name client_secret.json


---

## Protocol Used

The program uses **People API** , not CardDAV

---

## Supported Windows 10 Mobile Builds

The application supports the following **Windows 10 Mobile builds**:

* **1607**
* **1703**
* **1709**

 Background task syncs contacts from Google to phone every 15 mins in addition to manual sync.

---

## Dependencies

The application requires the following packages:

* `Microsoft.NET.Native.Framework.1.7`
* `Microsoft.NET.Native.Runtime.1.7`
* `Microsoft.VCLibs.140.00`

---

## Notes

## Screenshot
<p align="center">
  <img src="docs/images/screen.png" width="320">
</p>

---
