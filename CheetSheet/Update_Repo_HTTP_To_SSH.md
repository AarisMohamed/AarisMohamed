# Make Sure Your GitHub Repo Uses SSH Instead of HTTPS

### Your repository may still be using HTTPS, which asks for credentials. To check, run:

`git remote -v`

#### If you see:

`origin  https://github.com/your-username/your-repo.git (fetch)`


`origin  https://github.com/your-username/your-repo.git (push)`

👉 You need to switch it to SSH.


# Change Repository URL to SSH

### Run this command to update your repository remote to SSH:

`git remote set-url origin git@github.com:your-username/your-repo.git`

### Now, check again with:

`git remote -v`

#### You should see:

`origin  git@github.com:your-username/your-repo.git (fetch)` 

`origin  git@github.com:your-username/your-repo.git (push)`


# Test SSH Authentication

### Make sure your SSH connection to GitHub is working:

`ssh -T git@github.com`

#### If it works, you'll see:
✅ "Hi your-username! You've successfully authenticated..."
