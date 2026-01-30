# Setup Instructions for Your GitHub Profile with Pacman Contribution Graph

Follow these steps to set up your GitHub profile README with the animated Pacman contribution graph:

## Step 1: Create the Profile Repository

1. Go to GitHub: https://github.com/new
2. **Repository name MUST be exactly:** `DulajDil` (same as your username)
3. Make it **Public**
4. ✅ Check "Add a README file"
5. Click "Create repository"

## Step 2: Upload the Files

You have two options:

### Option A: Using GitHub Web Interface (Easier)

1. Go to your new repository: https://github.com/DulajDil/DulajDil
2. Click "Add file" → "Upload files"
3. Drag and drop the `README.md` file from the `DulajDil-profile` folder on your Desktop
4. Commit the changes

5. Create the GitHub Actions workflow:
   - Click "Add file" → "Create new file"
   - In the filename field, type: `.github/workflows/pacman.yml`
   - Copy the contents from the `pacman.yml` file in your Desktop folder
   - Commit the file

### Option B: Using Git Command Line

1. Open Terminal and navigate to the folder on your Desktop:
   ```bash
   cd ~/Desktop/DulajDil-profile
   ```

2. Initialize git and push to GitHub:
   ```bash
   git init
   git add .
   git commit -m "Initial commit with Pacman contribution graph"
   git branch -M main
   git remote add origin https://github.com/DulajDil/DulajDil.git
   git push -u origin main
   ```

## Step 3: Run the Workflow

1. Go to your repository: https://github.com/DulajDil/DulajDil
2. Click on the "Actions" tab
3. Click on "generate pacman game" workflow on the left
4. Click "Run workflow" button (on the right)
5. Click the green "Run workflow" button in the dropdown
6. Wait about 1-2 minutes for it to complete

## Step 4: Check Your Profile!

1. Go to your profile: https://github.com/DulajDil
2. You should now see the animated Pacman eating your contributions!

## Troubleshooting

- **Workflow not running?** Make sure the repository is public and the workflow file is in `.github/workflows/pacman.yml`
- **Pacman not showing?** Wait a few minutes after the workflow completes, then refresh your profile
- **SVG not found?** Make sure the workflow completed successfully and created the `output` branch

## Customization

You can customize the README.md file with:
- Your bio and information
- Technologies you use
- GitHub stats widgets
- Links to your social media
- Projects you're working on

The Pacman graph will automatically update every 24 hours with your latest contributions!

---

Need help? Check the original project: https://github.com/abozanona/pacman-contribution-graph
