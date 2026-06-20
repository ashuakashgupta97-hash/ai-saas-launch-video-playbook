# GitHub Upload Guide For First-Time Users

This guide assumes you have never uploaded a project to GitHub before.

## Option A: Upload Through GitHub Website

This is the easiest method.

### Step 1: Create A GitHub Account

Go to:

```text
https://github.com
```

Create an account or sign in.

### Step 2: Create A New Repository

1. Click the `+` icon in the top-right.
2. Click `New repository`.
3. Repository name suggestion:

```text
ai-saas-launch-video-playbook
```

4. Add description:

```text
A practical playbook for creating AI-assisted SaaS launch videos using scripting, HyperFrames, voiceover, subtitles, and QA.
```

5. Choose `Public`.
6. Do not add a README from GitHub because this folder already has one.
7. Click `Create repository`.

### Step 3: Upload Files

1. In the empty repository, click `uploading an existing file`.
2. Drag and drop all files and folders from this local folder:

```text
C:\Users\<your-name>\Documents\AI SaaS Launch Video Playbook
```

3. Wait for upload to finish.
4. Add commit message:

```text
Initial public playbook
```

5. Click `Commit changes`.

## Option B: Upload Using GitHub Desktop

This is also beginner-friendly.

### Step 1: Install GitHub Desktop

Download from:

```text
https://desktop.github.com
```

### Step 2: Sign In

Open GitHub Desktop and sign in with your GitHub account.

### Step 3: Add Existing Repository

1. Click `File`.
2. Click `Add local repository`.
3. Select:

```text
C:\Users\<your-name>\Documents\AI SaaS Launch Video Playbook
```

4. If it says it is not a Git repository, choose `create a repository`.

### Step 4: Publish

1. Add a commit message:

```text
Initial public playbook
```

2. Click `Commit to main`.
3. Click `Publish repository`.
4. Keep it public if you want people to find it.

## Option C: Upload Using Command Line

Use this only if you are comfortable with terminal commands.

```powershell
cd "C:\Users\<your-name>\Documents\AI SaaS Launch Video Playbook"
git init
git add .
git commit -m "Initial public playbook"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/ai-saas-launch-video-playbook.git
git push -u origin main
```

Replace `YOUR_USERNAME` with your GitHub username.

## Recommended Repository Settings

After upload:

1. Go to repository page.
2. Click the gear icon beside `About`.
3. Add topics:

```text
ai
saas
video
motion-graphics
hyperframes
product-launch
prompt-engineering
business-transformation
```

4. Add a short website or portfolio link if you have one.

## Suggested LinkedIn Post

```text
I built a reusable playbook for creating AI-assisted SaaS launch videos.

The repo covers:
- turning a business use case into a video brief
- writing a concise product story
- mapping narration to scenes
- using HyperFrames for motion graphics
- syncing voiceover and subtitles
- anonymizing internal product examples
- exporting short clips for portfolio use

The example is a generic email order intake platform, but the workflow can be adapted to any internal AI tool, workflow automation, or enterprise SaaS product.
```
