<p style="text-align:center;"><em>This project has been created as part of the 42 curriculum by jmagand</em></p>

<h1 style="text-align:center;"> <strong> NetPractice </strong></h1>

<details>
<summary><strong><font color="orange">🔎 Description</font></strong></summary>
<div> <br>
 This project involves solving networking problems to make a network function properly. <br><br>
 There are 10 levels available for training. Below is an example: <br>
 <p align=center> <img src="img/lvl9.png" alt="level 9" width=75%/> </p> <br>
 <br>For each level, a non-functioning network diagram is displayed. Your job is to fix it.
</div>
</details>
<br><br>

<details>
<summary><strong><font color="orange"> 📖 Instructions</font></strong></summary>
Here you'll find revelant information about how to install the project and how does it work.
<div>
<br>

<details>
 <summary><strong>📋 Installation</font></strong></summary>
 <div> <br>
<strong> • Download </strong> the file attached to the project’s page. <br>
<strong> • Extract </strong> the files into any folder of your choice. <br>
<strong> • Run </strong> the run.sh file. This shell script will launch a web server and
open your preferred web browser to the dedicated page. You also can just drag it on your web browser. <br><br>
<strong> This interface should open in your web browser: <br> </strong>
<p align=center> <img src="img/welcome.png" alt="sign-in form" width=50%/> </p> <br>
You can practice by entering your login in the field to use your personal configuration. <br>
Alternatively, you can use the "evaluation" tab to generate a random configuration, also suitable for evaluations.
</div>
</details> <br>

<details>
 <summary><strong>❓ How does it works</font></strong></summary> <br>
<div> <br>
 At the top of your window, you will see one or more objectives that you must achieve by
 adjusting the available configuration so that the network functions properly. <br>
 <p align=center> <img src="img/quests.png" alt="goals of the exercisee" width=50%/> </p> <br>
 There are three buttons you can use: <br>
 <p align=center> <img src="img/buttons.png" alt="possible buttons" width=50%/> </p> <br>
<strong> • [Check again]</strong> to verify whether your configuration is correct. <br>
<strong> • [Get my config]</strong> to download your configuration. you will need it when submitting your assignment <br>
<strong> • [Next level]</strong> ⚠️ It will appear only if have successfully completed a level. Click this button to proceed to the next level. <br><br>
At the bottom of the page, you will see logs. They can help you understand why your
configuration is incorrect, for example, if a gateway is missing or an IP address is
invalid. <br>
<p align=center> <img src="img/logs.png" alt="logs of the actual configuration" width=50%/> </p> <br><br>
To succeed a level, modify the unshaded fields until your network configuration is correct. <br><br>
</div>
</details> <br>
<details>
 <summary><strong>⚠️ Submission details</font></strong></summary> <br>
<div> <br>
After suceed a level, make sure to get your config, because you've to export each level, from 1 to 10, into your repository's root. <br>
<p align=center> <img src="img/configurations.png" alt="configuration JSON level 1 to 10" width=50%/> </p> <br>

</details>
</details>
<br><br>


<details>
<summary><strong><font color="orange">ℹ️ Resources</font></strong></summary>
<div>
<br>
Contenu détaillé de la section 1. Le Markdown fonctionne généralement à l'intérieur.
</div>
</details>

<br><br>
<font color="orange">⚠️ Attention à ce point</font>



<div align="center">

✨ **NetPractice** ✨<br>
<sub><em>42 Network Configuration Trainer</em></sub>

</div>

---

### 🎯 **Project Overview**
<p align="center">
<em>Created as part of the 42 curriculum by <strong>jmagand</strong></em>
</p>

This project is a **network configuration simulator** where you solve networking problems to make virtual networks function properly. With **10 progressive levels**, you'll diagnose and fix misconfigured networks through a practical web interface.

---

## 📋 **Table of Contents**
- [🔍 **Description**](#-description)
- [📖 **Instructions**](#-instructions)
  - [🚀 Installation](#-installation)
  - [⚙️ How It Works](#️-how-it-works)
  - [📤 Submission Details](#-submission-details)
- [📚 **Resources**](#-resources)
- [⚠️ **Important Notes**](#️-important-notes)

---

## 🔍 **Description**
This project involves solving networking problems to make a network function properly.

**Key Features:**
- **10 training levels** of increasing complexity
- **Visual network diagrams** with interactive configuration
- **Real-time feedback** through system logs
- **Configuration export** for assignment submission

**Example Level Preview:**
<p align="center">
<img src="img/lvl9.png" alt="Level 9 Network Diagram" width="85%"/>
<sub><em>Example of a network configuration challenge</em></sub>
</p>

For each level, you're presented with a **non-functioning network diagram** and must adjust configurations until all connections work correctly.

---

## 📖 **Instructions**
### 🚀 **Installation**
**Step-by-Step Setup:**
1. **Download** the file attached to the project's page
2. **Extract** the files into any folder of your choice
3. **Run** the `run.sh` file:
   ```bash
   ./run.sh


   Expected Result:
<p align="center"> <img src="img/welcome.png" alt="NetPractice Welcome Screen" width="70%"/> <sub><em>Welcome interface after successful launch</em></sub> </p>

Access Options:

    Practice Mode: Enter your login to use personal configurations

    Evaluation Mode: Generate random configurations suitable for evaluations

⚙️ How It Works

Interface Layout:
<p align="center"> <img src="img/quests.png" alt="Level Objectives Display" width="70%"/> <sub><em>Objectives displayed at the top of each level</em></sub> </p>

Control Buttons:
<p align="center"> <img src="img/buttons.png" alt="Control Buttons" width="60%"/> <sub><em>Primary interface controls</em></sub> </p>
Button	Function	Availability
Check again	Validates your current configuration	Always available
Get my config	Downloads configuration file for submission	Always available
Next level	Advances to next challenge	Only appears after successful completion

Diagnostic Tools:
<p align="center"> <img src="img/logs.png" alt="Configuration Logs" width="70%"/> <sub><em>Diagnostic logs helping identify configuration errors</em></sub> </p>

The bottom log panel provides real-time feedback about:

    Missing gateways

    Invalid IP addresses

    Routing issues

    Connectivity problems

Gameplay Flow:

    Examine the network diagram and objectives

    Modify the editable (unshaded) configuration fields

    Check your configuration using the validation button

    Review logs to understand any failures

    Repeat until all objectives are met

    Export your configuration when successful

📤 Submission Details

Important Submission Requirements:

    Complete all 10 levels successfully

    Export each level's configuration using the "Get my config" button

    Save all configuration files (level1.txt through level10.txt) in your repository's root directory

Expected Repository Structure:
<p align="center"> <img src="img/configurations.png" alt="Configuration Files Structure" width="60%"/> <sub><em>Required configuration files for submission</em></sub> </p>
📚 Resources

Helpful References:

    📘 IP Addressing & Subnetting - Understanding network fundamentals

    🔗 TCP/IP Protocols - Core networking concepts

    🛠️ Network Troubleshooting - Systematic debugging approaches

    💡 Common Configuration Errors - Typical mistakes and solutions

Pro Tips:

    Start simple - Ensure basic connectivity before complex routing

    Read logs carefully - They often pinpoint the exact issue

    Validate incrementally - Check after each significant change

    Document your approach - Helps with debugging and learning