# Slack Agent

Slack Agent is an AI-powered Slack assistant designed to enhance team communication, project management, and task automation. It integrates with **Slack**, **Trello**, **Google APIs (Gmail, Docs, Sheets)**, and leverages **OpenAI API** for core natural language tasks with **Gemini API** as a fallback model. 

This assistant is capable of:
- Fetching Trello credentials and card details on request
- Sending humanlike emails directly from Slack
- Automating team reminders for Namaz times
- Providing interactive elements in Slack via block models (buttons)
- Running **4 n8n workflows** with built-in **error handling** and **human-in-the-loop** oversight

---

## Features

### 1. **Trello Card Retrieval**
   - Fetch credentials from **Trello cards** using a **scraper** function. The system only retrieves the information that is requested (e.g., credentials or specific details), preventing unnecessary data access.
   - Automatically formats Trello card data into structured formats to improve project management and team coordination.

   **Trello Scraper Workflow**:
   - On request, the assistant fetches the **Trello card credentials** (e.g., card names, labels, due dates, and custom fields).
   - Only the required fields are retrieved to ensure minimal access and efficient processing.

### 2. **Email Sending**
   - The assistant allows you to send **humanlike emails** directly from Slack.
   - It integrates with **Gmail API**, enabling easy and fast communication without switching between platforms.
   - The **human-in-the-loop** approach ensures that all emails sent are monitored for accuracy.

### 3. **Interactive Slack UI**
   - Utilizes **Slack’s block models** to create interactive elements such as **buttons** for seamless engagement and task execution within Slack.
   - The assistant’s interface ensures ease of use and a smooth user experience.

### 4. **Namaz Time Reminders**
   - Sends personalized reminders to users for **Namaz times**, based on their presence within Slack.
   - The system dynamically detects the active users at specific times and sends reminders according to the **API-provided prayer times**.

### 5. **Error Handling**
   - Includes robust **error handling** within the workflows, ensuring that any issues or failures are caught and managed properly.
   - Notifications are sent to a designated user (or group) for immediate action or awareness.

### 6. **Workflows & Automation (n8n)**
   - The assistant is powered by **n8n workflows**, automating the processes for email sending, card creation, and Namaz time reminders.
   - The system includes **4 separate n8n workflows**, each dedicated to specific tasks.
   - **Human-in-the-loop monitoring** is embedded in the workflows, particularly for email verification.
