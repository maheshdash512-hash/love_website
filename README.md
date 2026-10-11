# A Little Love Website ❤️

A responsive romantic website built with Python and Flask. It includes your photo,
a love quote, floating hearts, a surprise message, and a gentle original melody
generated in the browser (no external song file needed).

## 1. Run it on Windows

Install Python 3.10+ from https://www.python.org/ if needed.

Open a terminal in this folder and run:

```bash
python -m venv venv
venv\Scripts\activate
pip install -r requirements.txt
python app.py
```

Open http://127.0.0.1:5000 in your browser. The tune starts only after you press
the play button because browsers require a user gesture before audio can play.

## 2. Personalize it

- Replace `static/girlfriend.jpg` with another photo if you wish. Keep the same filename.
- Edit the quote and surprise message in `templates/index.html`.
- The provided photo is stored locally in this project; consider whether you and
  your girlfriend are comfortable sharing it publicly before deploying.

## 3. Deploy on Render

1. Create a GitHub repository and upload the project files.
2. Sign in at https://render.com/ and create a new **Web Service** from that repository.
3. Set **Build Command** to `pip install -r requirements.txt`.
4. Set **Start Command** to `gunicorn app:app`.
5. Deploy and open the public URL Render provides.

Free-tier availability and behavior may change. If you make the repository public,
the photo in it may be publicly accessible; even with a private repository, the
deployed website and its photo are visible to anyone who has the website URL.
