# Anya Chatbot

## 📜 Project Origins
This chatbot was created in a joint partnership between Cal State LA Computer Science Senior Capston Project of 2024 and the Santa Barbara Public Defender's Office IT Team. The vision was to
leverage up and coming technologies to further build out a infrastructure with existing applications and automations devloped in the Power Platform, more specifically the Office's environment.
While current projects use the microsoft cloud technologies, like M365, Power Apps, Power Automate, Power BI, this project aimed to use an emerging technology to get ahead of the curve, that
is Microsoft Co-pilot.

---

## 🏗️ Project Structure
As it stands, the students referenced the existing applications and sharepoint lists that currently live in the county's Tenant to develop the chatbot. Unfortunately, Microsoft Co-pilot
studio is required to do any further development. Also unfortunately, a connection is not available to the county at the time of this repository's first commit. This being the
Microsoft TranslatorV2 connector. As a result the project contains 2 folders and the original solution. the repo folder is the solution unpacked using the Power Platform CLI tools, while source contains slightly
edited version of the unpacked files. Surgicaly the references and flow with the trouble connector have been removed and repackaged into the Agent_Clean.zip found in source. Using the connection refrerences found
the connections were made in the solution explorer of the power platform to successfully import the cleaned version of the agent. If in the future access is gained for the MicrosoftTranslatorV2, then import the original solution,
and everything should work as intended.

---

## 🛠️ Source Extraction Process
We use **Visual Studio Code** and the **Power Platform CLI (PAC)** to bridge the gap between the Power Apps Studio and our local development environment.

### 1. Prerequisites
* [VS Code](https://code.visualstudio.com/) installed.
* **Power Platform CLI Extension** installed from the VS Code Marketplace.
* The `.zip` file provided by the students to unpack.

### 2. Extraction (Unpacking)
To extract the source files for version control, open your terminal in the project root and run the following command. 

> **Note:** We use double quotes to handle file paths that contain spaces.

```powershell
pac solution unpack -z D:\Practice\CLI\Solution_1_0_0_0.zip -f D:\Practice\CLI\Solution_1_0_0_0.zip
```
