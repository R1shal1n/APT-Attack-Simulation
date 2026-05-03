# Charming Kitten APT Adversary Simulation


This is a simulation of an attack by the APT group **Charming Kitten**, targeting multiple sectors including government, military, and critical infrastructure across the Middle East. The group’s targeting has expanded beyond government entities to include the maritime, aviation, and financial sectors, reflecting a growing interest in regional logistics and critical economic infrastructure.

<img width="1146" height="636" alt="imageedit_3_7755177569" src="https://github.com/user-attachments/assets/81ea1f39-68e1-45b5-89dd-77137734a8c4" />

Recent campaigns have targeted entities in Egypt, Saudi Arabia, the UAE, Turkey, Hungary, Turkmenistan, Israel, and South America. These attacks demonstrate the group’s ability to pivot between sectors while conducting multiple operations simultaneously. The campaign was active throughout 2025 and 2026. This simulation is based on research from 

Palo Alto Unit 42:
[https://unit42.paloaltonetworks.com/boggy-serpens-threat-assessment/](https://unit42.paloaltonetworks.com/boggy-serpens-threat-assessment/)

and Group-IB: https://www.group-ib.com/blog/muddywater-operation-olalampo/

<img width="1262" height="700" alt="word-image-341009-175304-1-1262x700" src="https://github.com/user-attachments/assets/78362455-3c93-4a60-88ec-6132d407f166" />


The attack group delivered a malicious Excel and Word files designed to mimic the target’s internal financial records. The lure appeared as a legitimate spreadsheet containing payment details and cash flow projections.

The infected document included specific references to “Engineering, Construction & Marine Services” and used local currency (AED), along with realistic transaction descriptions such as “Payroll Payments via WPS,” making it highly convincing to the target.

<img width="897" height="483" alt="Screenshot 2026-05-03 at 05-44-34 Boggy Serpens Threat Assessment" src="https://github.com/user-attachments/assets/b7e58230-ed40-4061-9896-a992c7e7336b" />



In this campaign, the blurred document lure delivers a new payload  as a custom HTTP backdoor.

To maintain persistence, the group has evolved its development approach by leveraging AI-generated code and Rust-based tools, such as the BlackBeard backdoor, to rapidly deploy custom implants. Additionally, the group uses standard HTTP status codes, customized UDP based traffic, and the Telegram API for  C2 communications.
