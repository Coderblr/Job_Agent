**Job Agent**
================

A Python-based job agent designed to help job seekers automate their job search process.

**Overview**
------------

This project is a simple yet effective tool that allows users to manage multiple job boards and receive
notifications when new jobs match their specified criteria. The agent uses web scraping techniques to monitor job
postings on various platforms, making it easier for users to stay up-to-date with the latest job opportunities.

**Features**
------------

*   **Multi-job board support**: Currently supports [Job Board 1](https://www.jobboard1.com/), [Job Board
2](https://www.jobboard2.com/), and [Job Board 3](https://www.jobboard3.com/) (add more job boards as needed)
*   **Customizable job criteria**: Users can set specific filters to match their desired job types, locations, and
industries.
*   **Notification system**: Receives notifications when new jobs that match the user's criteria become available.

**Installation**
---------------

To use this project, follow these steps:

1.  Clone the repository using Git: `git clone https://github.com/Coderblr/Job_Agent.git`
2.  Install required libraries by running: `pip install -r requirements.txt`

**Usage**
-----

### Step 1: Configure job boards and credentials

Create a file named `job_board_config.json` in the project root directory with the following structure:
```json
{
    "board1": {
        "url": "https://www.jobboard1.com/",
        "username": "your_username",
        "password": "your_password"
    },
    "board2": {
        "url": "https://www.jobboard2.com/",
        "username": "your_username",
        "password": "your_password"
    },
    ...
}
```
Replace `your\_username` and `your\_password` with your actual credentials for each job board.

### Step 2: Set up notifications

Create a file named `notification_settings.json` in the project root directory:
```json
{
    "notification_interval": 300, // in seconds (e.g., 5 minutes)
    "notification_type": "email"
}
```
Replace `notification\_interval` with your desired notification interval and `notification\_type` with either
"email" or "slack".

### Step 3: Run the job agent

Run the following command to start the job agent:
```bash
python main.py
```
The job agent will begin monitoring job boards and sending notifications according to your settings.

**License**
---------

This project is licensed under the [MIT License](https://opensource.org/licenses/MIT).

**Contributing**
--------------

Contributions are welcome! If you'd like to contribute to this project, please fork this repository and submit a
pull request.
