# AI Neural Style Transfer

A Flask application that applies artistic style transfer using the AdaIN model.

## Run locally

From the `NST_Code` directory:

```bash
pip install -r ../requirements.txt
python app.py
```

Then open `http://localhost:5000`.

## Deploy on Render

Create a Render **Web Service** connected to this repository with:

- **Root Directory:** `NST_Code`
- **Build Command:** `pip install -r ../requirements.txt`
- **Start Command:** `gunicorn --bind 0.0.0.0:$PORT app:app`

The free Render service is suitable for a demo, but it sleeps after inactivity and
its local filesystem is temporary. Uploaded and generated images should therefore
not be treated as permanent storage.

## Attribution

This project is based on the AI Neural Style Transfer project from the
Apna College course and the original repository:

https://github.com/shradha-khapra/ai-nst-project

Deployment configuration and production-related fixes were added by Kunal Soni.
