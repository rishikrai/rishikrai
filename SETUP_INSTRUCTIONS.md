# How to Set Up Your GitHub Profile README

## Step 1: Create the special repository
1. Log in to GitHub as **rishikrai**.
2. Click the **+** icon (top right) → **New repository**.
3. Repository name: type your username **exactly** → `rishikrai`
   - This exact match is what tells GitHub to treat it as your profile repo.
4. Set visibility to **Public** (profile READMEs must be public to show).
5. Check **"Add a README file."**
6. Click **Create repository**.

## Step 2: Replace the README content
1. In your new `rishikrai` repo, click on `README.md`.
2. Click the pencil (✏️) icon to edit.
3. Delete the existing content.
4. Open `README.md` from this zip, copy everything, and paste it in.
5. Scroll down, add a commit message like "Update profile README," and click **Commit changes**.

## Step 3 (Optional): Add the live contribution snake animation
The README references a snake animation image. To make it actually reflect *your* contributions (not a generic example):
1. In your `rishikrai` repo, go to **Add file → Upload files**.
2. Upload the `.github/workflows/snake.yml` file from this zip, keeping the same folder path (`.github/workflows/snake.yml`).
   - Easiest way: use **Add file → Create new file**, name it `.github/workflows/snake.yml`, and paste in the contents.
3. Commit the file. This triggers a GitHub Action that generates the snake animation automatically once a day (and once immediately if you trigger it manually).
4. Go to the **Actions** tab in your repo → select **Generate Snake Animation** → click **Run workflow** to generate it right away.
5. Once it runs successfully, it creates an `output` branch containing the SVG. The README already points to a public example snake — if you want to swap it for **your own generated version**, update this line in `README.md`:
   ```
   <img src="https://raw.githubusercontent.com/platane/platane/output/github-contribution-grid-snake.svg" width="100%"/>
   ```
   Replace it with:
   ```
   <img src="https://raw.githubusercontent.com/rishikrai/rishikrai/output/github-contribution-grid-snake.svg" width="100%"/>
   ```

## Step 4: Verify it worked
1. Go to `github.com/rishikrai` (your profile page).
2. Your new README should now appear at the top of your profile.
3. Give it a minute or two — some badges (stats, streak, profile views) may take a short time to populate.

## Step 5: Personalize the placeholders
Before showing this off, go back into `README.md` and:
- Replace the **3 placeholder projects** with your real repos (name, description, tech, and optionally a screenshot image linked to the repo).
- Add a portfolio/website badge later if you build one — just add this line near the LinkedIn badge:
  ```
  [![Portfolio](https://img.shields.io/badge/Portfolio-000000?style=for-the-badge&logo=vercel&logoColor=white)](YOUR_URL_HERE)
  ```

That's it — your profile is live!
