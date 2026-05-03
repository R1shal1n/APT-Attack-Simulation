# Charming Kitten APT Adversary Simulation


This is a simulation of an attack by the APT group **Charming Kitten**, targeting multiple sectors including government, military, and critical infrastructure across the Middle East. The group’s targeting has expanded beyond government entities to include the maritime, aviation, and financial sectors, reflecting a growing interest in regional logistics and critical economic infrastructure.

<img width="1672" height="941" alt="e48cc470-d701-45fd-ba6a-a1cfe6552bcd" src="https://github.com/user-attachments/assets/7888b72d-8991-4b4a-aedf-3cfeb800b17d" />


Recent campaigns have targeted entities in Egypt, Saudi Arabia, the UAE, Turkey, Hungary, Turkmenistan, Israel, and South America. These attacks demonstrate the group’s ability to pivot between sectors while conducting multiple operations simultaneously. The campaign was active throughout 2025 and 2026. This simulation is based on research from 

Palo Alto Unit 42:
[https://unit42.paloaltonetworks.com/boggy-serpens-threat-assessment/](https://unit42.paloaltonetworks.com/boggy-serpens-threat-assessment/)

and Group-IB: https://www.group-ib.com/blog/muddywater-operation-olalampo/

<img width="1262" height="700" alt="word-image-341009-175304-1-1262x700" src="https://github.com/user-attachments/assets/78362455-3c93-4a60-88ec-6132d407f166" />

In this campaign, the blurred document lure delivers a new payload  as a custom HTTP backdoor. To maintain persistence, the group has evolved its development approach by leveraging AI-generated code and Rust-based tools, such as the BlackBeard backdoor, to rapidly deploy custom implants. Additionally, the group uses standard HTTP status codes, customized UDP based traffic, and the Telegram API for C2 communications.

<img width="689" height="578" alt="Screenshot 2026-05-03 at 17-06-02 Operation Olalampo Inside MuddyWater’s Latest Campaign Group-IB Blog" src="https://github.com/user-attachments/assets/dc9ea0ba-0c97-42ff-af21-fb6ab4f8c28c" />

## The first stage (delivery technique)

The initial campaign targeted project engineers using industry-specific terminology for subsea pipelines. The lure document was blurred in order to deceive targets into clicking “Enable Content” thereby triggering the execution of the embedded macro.


<img width="1177" height="700" alt="word-image-353730-175304-5-1177x700" src="https://github.com/user-attachments/assets/3c5ea612-6b8c-4b75-bca0-f0df1a23c0d0" />


In another wave the attack group delivered a malicious Excel and Word files designed to mimic the target’s internal financial records. The lure appeared as a legitimate spreadsheet containing payment details and cash flow projections.

The infected document included specific references to “Engineering, Construction & Marine Services” and used local currency (AED), along with realistic transaction descriptions such as “Payroll Payments via WPS” making it highly convincing to the target.

<img width="897" height="483" alt="Screenshot 2026-05-03 at 05-44-34 Boggy Serpens Threat Assessment" src="https://github.com/user-attachments/assets/b7e58230-ed40-4061-9896-a992c7e7336b" />




