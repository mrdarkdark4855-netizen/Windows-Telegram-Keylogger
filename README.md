Cross-Platform Input Monitor Lab
An educational Python project designed to explore OS-level event listening and external API communication. The script captures keyboard events locally and transmits the batched text data over to a private Telegram channel via a bot interface.

---

🛠️ System Architecture
The project relies on a local event listener that hooks into the operating system's input stream, batches the data to avoid API rate limits, and securely transmits it over HTTPS.



---

🚀 Features & Learning Outcomes
Asynchronous Event Hooking: Utilized the pynput library to create a non-blocking background thread that actively listens to keyboard events.
Network Integration: Implemented the requests library to handle payload delivery to the Telegram Bot API endpoint.
Cross-Platform Architecture Hurdles: * Debugged and documented why Windows-specific libraries (like winreg and environment variables like %APPDATA%) fail natively inside Linux distributions like Kali.
Learned to adapt deployment strategies depending on the target environment's architecture.

---

📋 Prerequisites
To run this script locally, you need Python installed on your machine along with the following external dependencies:

```bash
pip install pynput requests
