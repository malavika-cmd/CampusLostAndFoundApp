# Campus Lost & Found App

## Overview
The Campus Lost & Found App is a centralized mobile application designed for reporting, searching, and claiming lost items around campus. College campuses are large, busy environments where personal items are frequently lost, and current solutions relying on social media posts or word of mouth are disorganized and inefficient. This application solves that problem by providing a quick, reliable way for students, faculty, and staff to recover lost belongings.

## Key Features

**User Authentication & Profiles**
* Users register securely using their university credentials (e.g., a valid `@vt.edu` address).
* Accounts are protected by password hashing and encrypted session management using JSON Web Tokens (JWT).
* Users can manage their personal profiles, including optional profile pictures and contact preferences.

**Reporting Workflows**
* **Report Lost Items:** Users can post lost items by providing a title, description, category, date lost, location last seen, and up to 5 optional photos.
* **Report Found Items:** Finders can list discovered items with similar detailed criteria and update the status between "Available" and "Claimed".

**Search, Matching, & Notifications**
* **Advanced Search:** Users can filter listings by category, item type (lost/found), location, date range, and status.
* **Item Matching:** The system analyzes tags, categories, text, and locations to provide a ranked list of recommended matching posts.
* **Real-Time Alerts:** The system sends timely notifications to users when a potential match for their item is found.

**Secure Claiming & Communication**
* **Proof of Ownership:** To claim an item, a user must submit verification, such as matching descriptions, unique identifiers, or photo evidence.
* **Claim Review:** Finders review the submitted proof and can confidently accept or decline the claim request.
* **In-App Messaging:** Users can securely communicate within a chat thread linked to the specific item post to coordinate pickups.

**Administration & Moderation**
* **Admin Dashboard:** Administrators can view real-time system analytics, including active items, successful returns, and server uptime.
* **Content Moderation:** Admins can delete or hide posts that violate community guidelines.
* **User Reports:** The system allows admins to review inappropriate behavior reports and take actions such as dismissing the report, warning the user, or suspending the account.

## Security & Architecture
* Data transmission is strictly secured using Transport Layer Security (TLS) 1.3 and SSL Certificate Pinning to prevent MITM attacks.
* Sensitive database fields are protected using AES-256-GCM encryption.
* Passwords are hashed using strong algorithms like bcrypt.
* Strict API rate limiting is enforced to defend against brute-force attempts and SQL injections.

## Team (Group 11)
* **Unnati Nettur:** Backend for Search, Matching & Communication.
* **Ally Plewniak:** Frontend + Backend for the Lost Items.
* **Malavika Saritha:** Frontend + Backend for the Found Items.
* **Dongjin Shin:** Frontend + Authentication Backend.
* **Taeoh Yi:** Front end for Admin and Backend for System Management.

## Repository
* **GitHub Link:** https://github.com/malavika-cmd/CampusLostAndFoundApp.git
