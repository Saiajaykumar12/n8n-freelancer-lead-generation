# 🤖 Automated Lead Generation from Freelancer.com

An n8n workflow that automatically fetches freelance project leads 
every hour and saves them to Google Sheets.

## 🔧 How It Works
1. Reads job titles from Google Sheets (Sheet1)
2. Filters only "pending" status rows
3. Calls Freelancer.com API with each job title
4. Parses project details (budget, skills, client, URL)
5. Saves leads to Sheet2 automatically
6. Updates status to "done" after each run

## 🛠️ Tech Stack
- n8n (workflow automation)
- Freelancer.com REST API
- Google Sheets API
- JavaScript (custom code node)

## 📊 Output Fields
| Field | Description |
|-------|-------------|
| Project_Title | Name of the project |
| Budget | Project budget in local currency |
| Skills_Required | Required tech skills |
| Client_Country | Where the client is from |
| Bid_Count | Number of bids already placed |
| Project_URL | Direct link to apply |

## 🚀 How to Use
1. Import the JSON file into your n8n instance
2. Connect your Google Sheets account
3. Add your Freelancer API token
4. Set up your job titles in Sheet1
5. Activate the workflow — runs every hour automatically!
