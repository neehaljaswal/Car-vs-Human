# Teachable Machine Image Classifier

## Add your model
1. In Teachable Machine, export your Image Project using **TensorFlow.js**.
2. Extract the downloaded ZIP.
3. Copy `model.json`, `metadata.json`, and every `.bin` weights file into this project's `my_model/` folder.
4. Keep the filenames and folder structure as exported. The site expects `./my_model/model.json` and `./my_model/metadata.json`.

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
