# GitHub Repository Setup Instructions

## Step 1: Create Repository on GitHub

1. Go to: https://github.com/new
2. Repository name: `alice-garden-restaurant` (or any name you prefer)
3. Choose **Public** or **Private**
4. **DO NOT** check "Initialize this repository with a README"
5. Click **"Create repository"**

## Step 2: Update Remote and Push

After creating the repo, replace `YOUR-REPO-NAME` with your actual repository name:

```bash
# Remove the old remote
git remote remove origin

# Add the new remote (replace YOUR-REPO-NAME with your actual repo name)
git remote add origin https://github.com/Will0177/YOUR-REPO-NAME.git

# Verify the remote
git remote -v

# Push your code
git push -u origin master
```

## Alternative: Using GitHub CLI (if installed)

If you have GitHub CLI installed (`gh`), you can create the repo directly:

```bash
# Install GitHub CLI (if not installed)
# macOS: brew install gh

# Authenticate
gh auth login

# Create repo and push
gh repo create alice-garden-restaurant --public --source=. --remote=origin --push
```

## Troubleshooting

If you get authentication errors:
- Use a Personal Access Token instead of password
- Generate token at: https://github.com/settings/tokens
- Use token as password when prompted

