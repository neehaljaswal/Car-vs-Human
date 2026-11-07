# Teachable Machine Image Classifier

## Model included
Your Teachable Machine export is already installed in `my_model/` (`model.json`, `metadata.json`, and `weights.bin`). Keep this folder intact when uploading the project to GitHub/Vercel.

The `my_model/` folder should look similar to:

```text
my_model/
  model.json
  metadata.json
  weights.bin
```

There may be more than one `.bin` file; include all of them.

## Run locally
Use a local web server (camera access usually does not work when opening `index.html` directly):
- VS Code: install/use the Live Server extension and choose **Open with Live Server**.
- Or run `python -m http.server 8000` in this folder, then open `http://localhost:8000`.

## Deploy to Vercel
1. Upload this folder to a GitHub repository.
2. In Vercel, choose **Add New → Project** and import that repository.
3. Framework preset: **Other**. Build command: leave blank. Output directory: `.`.
4. Deploy. Make sure `my_model/` and all model files are committed to the repository.

The deployed site uses HTTPS, which is required by most browsers for camera access.
