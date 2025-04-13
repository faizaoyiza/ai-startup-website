# Hands-On Git Project: Collaborative Website Development with Git and GitHub

## Project Overview
This project simulates a collaborative Git and GitHub workflow between two developers, **Tom** and **Jerry**. The goal is to demonstrate how multiple contributors can work on the same project using branches, staging, committing, pushing, and merging changes in a structured manner.

---

## Part 1: Setup and Initial Configuration

### 1. Install Git
### 2. Create a GitHub Repository
- Log in to your GitHub account.
- Click the `+` button at the top-right and select **New repository**.
- Name the repository: `ai-startup-website`.
- Initialize the repository with a `README.md` file.
- Click **Create repository**.
<img width="955" alt="Image" src="https://github.com/user-attachments/assets/45468bdc-f7cc-44a6-93ce-c5285869387b" />
### 3. Clone the Repository Locally
```bash

# Create a folder for the Git project
mkdir git-project
cd git-project
<img width="782" alt="Image" src="https://github.com/user-attachments/assets/4a77a3e5-f172-4a13-a926-1adab4b805cb" />
# Clone the GitHub repo into this directory
git clone https://github.com/your-username/ai-startup-website.git
cd ai-startup-website

 <img width="833" alt="Image" src="https://github.com/user-attachments/assets/6f972740-7d68-4d30-9ddc-d914f55773a1" />


## Part 2: Tom's Workflow

### 1. Create an `index.html` file
```bash
echo "This is the Admin creating an index.html file for Tom" > index.html
```
You can view index.html file created on GitHub here https://github.com/faizaoyiza/ai-startup-website/blob/main/index.html
### 2. Check Git Status and Stage Changes
```bash
git status
git add index.html
git status
```
<img width="938" alt="Image" src="https://github.com/user-attachments/assets/2191af09-1542-4d27-a173-da9093532dc5" />

### 3. Commit and Push Initial Change
```bash
git commit -m "This is my first commit"
git push origin main
```
<img width="788" alt="Image" src="https://github.com/user-attachments/assets/419fae50-91d6-457e-b69b-6cb8c3769d36" />
### 4. Create Tom's Branch and Add Navigation
```bash
git checkout -b update-navigation

# Modify index.html
# Add the following content to the file
# "This is Tom adding Navigation to the AI-website"
echo "This is Tom adding Navigation to the AI-website" >> index.html

# Stage and commit changes
git add index.html
git commit -m "Update navigation bar"
git push origin update-navigation

<img width="926" alt="Image" src="https://github.com/user-attachments/assets/6c25fffc-7fcf-48d6-be47-1ba5bfa382ec" />


## Part 3: Jerry's Workflow

### 1. Switch Back to Main and Pull Updates
```bash
git checkout main
git pull origin update-navigation
```
<img width="803" alt="Image" src="https://github.com/user-attachments/assets/fe7008cd-c9f1-41db-ae41-f97e819162be" />
### 2. Create Jerry's Branch and Add Contact Info
```bash
git checkout -b add-contact-info

### Modify index.html
### Add the following content to the file
### "This is Jerry adding contact information"
echo "This is Jerry adding contact information" >> index.html

### Stage and commit changes
git add index.html
git commit -m "Add contact information"
git push origin add-contact-info

<img width="944" alt="Image" src="https://github.com/user-attachments/assets/d3ba0762-6aff-4cff-ae11-a932dab34da4" />


## Part 4: Review and Merge

<img width="947" alt="Image" src="https://github.com/user-attachments/assets/8f07a7ad-959b-491f-bb13-eaa8dd4e9551" />



<img width="874" alt="Image" src="https://github.com/user-attachments/assets/804fe691-8987-47e6-a94e-9a514a994507" />



 URL to the GitHub repository:  https://github.com/faizaoyiza/ai-startup-website/tree/main
