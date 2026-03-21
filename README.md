# Green Nest Solutions — Website Deployment Guide

## What's in this folder

```
greennest/
├── index.html       ← Home page
├── services.html    ← Services page
├── contact.html     ← Contact & Book page
├── css/
│   └── style.css    ← All styling
├── js/
│   └── main.js      ← Navigation, form, animations
└── images/
    └── logo.png     ← ADD YOUR LOGO HERE (see Step 1)
```

---

## STEP 1 — Add your logo

Before uploading, save your Green Nest logo file as:
  `logo.png`
and place it inside the `images/` folder.

---

## STEP 2 — Set up your contact form (Formspree)

The enquiry form on the Contact page uses a free service called Formspree
to send messages to your email inbox. Here's how to activate it:

1. Go to https://formspree.io and click "Get Started Free"
2. Sign up with your email: Admin@greennestpropertysolutions.com
3. Click "New Form" and give it a name (e.g. "Green Nest Enquiries")
4. Copy the Form ID — it looks like: `xpwzlkqr`
5. Open `contact.html` in a text editor
6. Find this line:
      action="https://formspree.io/f/YOUR_FORM_ID"
7. Replace YOUR_FORM_ID with the ID you copied, e.g.:
      action="https://formspree.io/f/xpwzlkqr"
8. Save the file

That's it — all enquiries will arrive in your inbox automatically.

---

## STEP 3 — Create a GitHub account

1. Go to https://github.com
2. Click "Sign up"
3. Use any email address (your personal one is fine)
4. Choose a username (e.g. greennest-solutions)
5. Verify your email address

---

## STEP 4 — Create a new GitHub repository

1. Once logged in to GitHub, click the green "New" button (top left)
2. Name the repository: `greennest-website`
3. Set it to "Public"
4. Do NOT tick any of the initialise options
5. Click "Create repository"

---

## STEP 5 — Upload your website files to GitHub

You do not need to install anything. Use GitHub's web upload:

1. On your new repository page, click "uploading an existing file"
2. Drag and drop your ENTIRE greennest folder contents into the upload area
   (all HTML files, the css folder, js folder and images folder)
3. Scroll down and click "Commit changes"
4. Wait for the upload to complete

---

## STEP 6 — Connect GitHub to IONOS

Now you'll tell IONOS to pull your website files from GitHub.

### Option A — Using GitHub Pages (Free hosting, then point IONOS domain)

1. In your GitHub repository, click "Settings"
2. Click "Pages" in the left menu
3. Under "Source", select "Deploy from a branch"
4. Under "Branch", select "main" and click Save
5. GitHub will give you a URL like: https://yourusername.github.io/greennest-website
6. Your site is now live at that URL

### Pointing your IONOS domain to GitHub Pages:

1. Log in to your IONOS account at https://my.ionos.co.uk
2. Go to "Domains & SSL"
3. Click on your domain name
4. Click "DNS" or "Manage DNS"
5. You need to add/edit these records:

   TYPE    | HOST | VALUE
   --------|------|------------------------
   A       |  @   | 185.199.108.153
   A       |  @   | 185.199.109.153
   A       |  @   | 185.199.110.153
   A       |  @   | 185.199.111.153
   CNAME   | www  | yourusername.github.io

6. Back in GitHub → Settings → Pages → Custom domain
7. Enter your domain: www.greennestpropertysolutions.com
8. Tick "Enforce HTTPS"
9. DNS changes take up to 24 hours to fully propagate

---

## STEP 7 — Making updates to your site in future

Whenever you want to change anything on the site:

1. Edit the relevant HTML or CSS file on your computer
2. Go to your GitHub repository
3. Click on the file you want to update
4. Click the pencil (edit) icon
5. Paste your updated content
6. Click "Commit changes"
7. Your site updates automatically within a few minutes

---

## Need help?

Call: 07729 247495
Email: Admin@greennestpropertysolutions.com
WhatsApp: https://wa.me/447729247495
