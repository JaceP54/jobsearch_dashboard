Job Search Dashboard (Flask + API + CSV Export)
A responsive web app built with Flask that allows users to search for remote tech jobs using real-time data from the RemoteOK API. Users can enter keywords, view job listings, and download matching results as a CSV file.

Features
Keyword-based job search (e.g., “python”, “developer”, “frontend”)

Live data fetched from RemoteOK.com

Clean, styled results dashboard

CSV export of search results

User-friendly navigation with “Back to Search” functionality

Tech Stack
Python (3.10+)

Flask (backend framework)

HTML + CSS (custom styling)

Jinja2 templates

Pandas

Requests

RemoteOK API

Project Structure
bash
Copy
Edit
jobsearch_dashboard/
│
├── app.py                  # Main Flask application
├── scraper.py              # API fetching and filtering logic
├── templates/
│   ├── index.html          # Homepage with search form
│   └── results.html        # Page displaying job results
├── static/
│   └── style.css           # Custom CSS for styling
├── jobs_<keyword>_<date>.csv  # Downloadable search results
 How It Works
User enters a keyword on the homepage

Flask passes the input to the scraper

Matching jobs are fetched and displayed

User can optionally download the results as a CSV

 Next Steps / Ideas
Add filters (e.g., location, tags, salary)

Allow favoriting or saving jobs

Deploy with Railway, Render, or Vercel

Add form validation and error handling