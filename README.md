🎓 GradPathway

GradPathway is a web application that helps international students discover potential master’s programmes worldwide.
Students can upload their undergraduate transcript (or enter GPA/degree details) and receive programme recommendations based on eligibility and preferences such as country or field of study.

This project was built as part of my Backend Engineering Capstone Project, using Django and Django REST Framework (DRF).




🚀 Features

User Accounts → Register, log in, and manage profile (with preferred countries)

Transcript Submission → Upload transcript files or manually enter GPA/degree information

Programme Search → Browse and search by programme, university, country, or discipline

Programme Matching Engine → Rule-based engine that recommends programmes based on eligibility

Programme Details → View description, tuition, duration, mode, and application link

Favourites → Save and manage favourite programmes

Admin Panel → Add, update, and delete universities/programmes

Authentication & Permissions → Token-based authentication for secure API usage




📡 External API Integration

College Scorecard API (U.S. Department of Education) → provides structured data on U.S. universities and graduate programmes (tuition, location, outcomes)

Non-U.S. universities → supported via manually seeded sample data




🛠️ Tech Stack

Backend: Django, Django REST Framework

Database: MySQL

Authentication: DRF Token Authentication

Documentation: DRF 



📂 Project Structure
gradpathway/
│
├── accounts/         # Custom user model & authentication
├── catalog/          # Universities & Programmes
├── transcripts/      # Transcript upload & storage
├── matches/          # Matching engine logic
├── favourites/       # Favourites feature
├── gradpathway/      # Core settings & configs
└── requirements.txt




🔑 API Endpoints (Examples)
🔐 Authentication

POST /api/auth/register/ → Register a new user

POST /api/auth/login/ → Obtain token

🎓 Programmes

GET /api/programmes/ → List/search programmes

GET /api/programmes/<id>/ → Retrieve programme detail

📄 Transcripts & Matching

POST /api/transcripts/ → Submit transcript

POST /api/matches/ → Create match request

GET /api/matches/<id>/results/ → Get match results

⭐ Favourites

POST /api/favourites/ → Add favourite

DELETE /api/favourites/<id>/ → Remove favourite
