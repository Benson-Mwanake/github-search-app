# GitHub Search App

A simple, responsive web application that allows users to search for GitHub profiles and view their public repositories. Built using **HTML**, **CSS**, and **JavaScript**, and powered by the **GitHub REST API**.

---

## Features

* Search for GitHub users by username
* View a list of matching profiles with avatars and profile links
* Click any user to load their public repositories
* Clean and responsive UI
* Built with vanilla JavaScript — no frameworks required

---

## Demo

Enter a GitHub username in the search bar and press **Submit**. The app will display:

* Matching GitHub users on the left
* The selected user's repositories on the right

---

## Project Structure

```
/
├─ index.html
├─ index.css
└─ js/
   └─ index.js
```

---

## 🛠️ How It Works

### 1. User Search

When the form is submitted, the app requests:

```
https://api.github.com/search/users?q={query}
```

It displays the results with:

* Avatar
* Username
* Link to GitHub profile

Clicking a username fetches their repositories.

### 2. Fetching Repositories

Once a user is clicked, the app fetches:

```
https://api.github.com/users/{username}/repos
```

Each repository is displayed as a clickable link.

---

## Installation & Setup

1. Clone the repository:

```bash
git clone git@github.com:Benson-Mwanake/github-search-app.git
```

2. Navigate into the project folder:

```bash
cd github-search-app
```

3. Open the project in your browser:

```bash
open index.html
```

No additional setup required.

---

## Technologies Used

* HTML5
* CSS3
* JavaScript (ES6)
* GitHub REST API v3

---

## Notes

* The GitHub API limits the number of unauthenticated requests.
* If results stop loading, wait a bit or authenticate using a GitHub token.

---

## Contribution Guidelines

Contributions are welcome! To contribute:

1. Fork the repository
2. Create a new feature branch
3. Commit changes with clear messages
4. Push to your fork and open a Pull Request

---

## License

**MIT License**

Copyright © 2025 **Benson Mwanake**

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

---

## Author

Developed by **Benson Mwanake**.
