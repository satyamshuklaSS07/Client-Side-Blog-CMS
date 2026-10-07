# PulseBlog — Client-Side Blog CMS

Client-Side Blog CMS based on the supplied project specification.

## Features
- Create, edit and delete posts
- Draft / Published status
- Status-based filtering
- Search posts
- Post preview
- Unique ID and timestamp
- Posts ordered by last updated
- Delete confirmation
- LocalStorage persistence
- Responsive animated UI
- Demo data

## Technologies
HTML5, CSS3, JavaScript, LocalStorage

## Run
Open `index.html` in VS Code and run it with Live Server, or open the file directly in a browser.

## Interview Questions

### 1. How would you differentiate draft and published posts?
Each post has a `status` property containing `draft` or `published`. The application uses it for badges and status filtering.

### 2. How would you implement editing an existing post?
Store the selected post ID, load its data into the form, then find that ID in the posts array and update its title, content, status and `updatedAt` timestamp.

### 3. How would you order posts by last updated?
Sort using `new Date(b.updatedAt) - new Date(a.updatedAt)` so the newest update appears first.
