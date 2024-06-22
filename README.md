# Discord Webhook Report Monitor

This script monitors a file named `miscmod_reports.dat` and sends a report-log to a specified Discord webhook. The script is designed to format the message and mention an admin role.

## Features

- Monitors `miscmod_reports.dat`.
- Formats the report with details about the reporter, reported player, and reason.
- Sends the report to a specified Discord webhook.
- Mentions an admin role in each message.
- Remembers the last processed line to avoid duplicate messages after restarting.

## Setup

1. **Install dependencies:**
    - This script requires the `requests` library. Install it using pip:
    ```sh
    pip install requests
    ```

2. **Configure the script:**
    - Open `report.py` and replace `your_webhook_url_here` with your Discord webhook URL.
    - Replace `admin_id_here` with the ID of the admin role you want to mention.

## Usage

1. **Run the script:**
    ```sh
    python report.py
    ```

2. **Output:**
    - It will monitor `miscmod_reports.dat` and send new reports to the specified Discord webhook.
