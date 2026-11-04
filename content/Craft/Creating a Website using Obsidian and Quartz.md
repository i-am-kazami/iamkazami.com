---
tags:
  - github
  - quartz
  - obsidian
  - technical
date: 2026-06-15
---
With the rise of social media and non customizable pages, I found that making your own little nook of the internet specifically contoured to your own tastes makes guests visiting feel like they stepped foot into your digital [[Homebase on the internet]].

Please support Jacky with this amazing project by supporting him on GitHub!
This post will cover how to create a static web app using Obsidian, Quartz, and GitHub Pages. 
This setup will allow you to write and quickly publish your blogs and projects using simple Markdown files.

What is Obsidian?

Obsidian is a markdown editor that allows you to link concepts between each other. For example, I am writing a topic about Tokyo which I can then link to a broader note about Japan.

What is Quartz?
Notes: Quartz is an open sourced project created by Jacky Zhao. https://quartz.jzhao.xyz/

Why not Obsidian Sync?
File size constraints
Recurring Costs
Low cost maintenance for students or anyone looking for a quick and simple way to get a website going.

Since we are using GitHub Pages which requires you to have your repository public, your entire Obsidian Vault will be readable by anyone. Please be careful to not publish any sensitive information and create a separate vault for your personal use. 

Overview

1. GitHub Configuration
2. Local build
3. Custom Domain (Optional)
4. Editing and Publishing

---

Purchase a Custom Domain Name
Add name servers
Point DNS records

Writing and Publishing
Setup Obsidian
CLI or GitHub Desktop
GitKraken or Other
### 0. (PreReq) Create a GitHub Account
Note, a GitHub Account can only host a single webpage using GitHub Pages. If you already have an account without Pages enabled, skip this step.
Navigate to https://github.com/ and create a free account using your preferred email.
## 1. Clone the Quartz Repository Locally
Navigate to Jacky Zhao's Quartz repository using this link https://github.com/jackyzha0/quartz

Click on the 'Use this template' button and select 'Create a new repository':



Name the repository to the domain name you purchased for the site. For example, if you purchased 'freedom.com' then enter that as the repo name. Select 'Public' or 'Private' depending on if you want your code to be readable to the public or not:



In your local computer, open CMD and run the command to login to authenticate through Github:
```
gh auth login
```
> Select HTTPS for the preferred protocol
> Authenticate Git with your GitHub credentials
> Authenticate with GitHub CLI through web browser

Enter your one time code to the browser that opened.
Navigate to the folder where you want the files to be located at and run the GitHub pull command to pull all the files locally:
```
git pull [Insert Your Repo Name Here]
```

You now have successfully integrated your Github repository locally.
## 2. Build the Application Locally
Navigate to where you Initialize the application 
```npm i```: 


Create the website ```npx quartz create```:



Build the application ```npx quartz build```:



Serve the website locally ``` npx quartz build --serve```:



Access the website using a web browser using ```http://localhost:8080/``` and you will see your locally run website appear:



You have successfully generated your static site and served it locally.
Any files should be saved into the /content folder. 
## 3. 

Select create when done GitHub Actions will now run when it detects a change in the repository.
## 3. Configure Github and DNS Settings


## 4. Editing Content in Your Site

### Setup Obsidian
You can download Obsidian at: 
### Setup Github Desktop
