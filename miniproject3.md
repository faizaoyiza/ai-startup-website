# Git Collaboration Simulation: AI Startup Website

This project demonstrates a Git collaboration simulation involving two team members — **Tom** and **Jerry** — working on separate features using Git branches, Pull Requests (PRs), and proper merging workflows via GitHub.

---

## 🛠️ Project Setup

- Repository: [`faizaoyiza/ai-startup-website`](https://github.com/faizaoyiza/ai-startup-website)
- Team Members:
  - **Tom:** Added a website footer
  - **Jerry:** Added social media links in the footer

---

## 👨‍💻 Tom's Workflow – Adding Footer

### 1. Created Feature Branch

bash
git checkout -b tom-update-footer

<img width="782" alt="Image" src="https://github.com/user-attachments/assets/fce31681-3c3d-4836-949a-a883ff916c7a" />
### 2. Made Changes in `index.html`

html
<footer>© 2025 AI Startup. All rights reserved.</footer>


### 3. Committed and Pushed Changes

bash
git add index.html
git commit -m "Tom added footer section to website"
git push origin tom-update-footer
<img width="896" alt="Image" src="https://github.com/user-attachments/assets/a3b923da-8b29-40ca-8ef5-ef1e74085abb" />

### 4. Created Pull Request (PR)

- **Base Branch:** `main`
- **Compare Branch:** `tom-update-footer`
- **PR Title:** `Add footer section to website`
- **PR Description:** `Tom added a footer with copyright info.`
<img width="949" alt="Image" src="https://github.com/user-attachments/assets/380d4249-32e0-44ca-947f-b2775af53be4" />
### 5. Merged PR into Main Branch

- Clicked **Merge pull request**
- Confirmed merge
<img width="931" alt="Image" src="https://github.com/user-attachments/assets/f9dd235d-bc00-4ada-9039-ba21e4bee940" />
---

## 🔁 Synchronizing `main` Branch

Before Jerry started work, the local `main` branch was updated:

```bash
git checkout main
git pull origin main
```

---

## 🧑‍💻 Jerry's Workflow – Adding Social Media Links

### 1. Created Feature Branch

bash
git checkout -b jerry-add-social-links
<img width="916" alt="Image" src="https://github.com/user-attachments/assets/f8674414-2a7e-4d81-8ac6-c53120ec4231" />

### 2. Updated `index.html`

```html
<div class="social-links">
  <a href="https://twitter.com/aistartup" target="_blank">Twitter</a> |
  <a href="https://linkedin.com/company/aistartup" target="_blank">LinkedIn</a>
</div>
```

### 3. Committed and Pushed Changes

```bash
git add index.html
git commit -m "Jerry added social media links to footer"
git push origin jerry-add-social-links
```
<img width="916" alt="Image" src="https://github.com/user-attachments/assets/f8674414-2a7e-4d81-8ac6-c53120ec4231" />
### 4. Created Pull Request (PR)

- **Base Branch:** `main`
- **Compare Branch:** `jerry-add-social-links`
- **PR Title:** `Add social media links to footer`
- **PR Description:** `Jerry added Twitter and LinkedIn links.`
<img width="919" alt="Image" src="https://github.com/user-attachments/assets/b15ebcaa-d1e0-4846-8b99-b095772ef788" />
### 5. Merged PR into Main Branch

- Clicked **Merge pull request**
- Confirmed merge

<img width="952" alt="Image" src="https://github.com/user-attachments/assets/c284c544-5413-4a45-99b6-ae50088ce7b6" />





