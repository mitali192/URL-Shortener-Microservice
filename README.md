# URL-Shortener-Microservice
A simple web app that shortens long URLs. Each link is assigned a unique Base62 code and stored in SQLite. Users can access the short URL to be redirected to the original.

Key Features:
- Form-based interface to submit long URLs.
- Generates compact, encoded short links.
- Stores and retrieves URL mappings from SQLite.
- Redirects short link to the original target.
- Supports full single-file implementation for deployment.

Technologies Used:
- Python 3.12
- Flask (Web framework)
- SQLite (Database)
- Base62 encoding (for short links)

File Structure:
- URLShortener.py → Single-file Flask application with logic for form, DB, redirect, and encode/decode.
- urls.db         → SQLite database for link storage.

How to Run:
1. Install Python 3.12 and Flask: `pip install flask`.
2. Run `python URLShortener.py`.
3. Open browser and visit: `http://localhost:5000/`.

Future Enhancements:
- Admin dashboard to view/manage all shortened links.
- Add click analytics and expiration settings.
- Add custom alias feature.
- Deploy on cloud with domain and SSL.
