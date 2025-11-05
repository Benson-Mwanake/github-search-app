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
git clone https://github.com/your-username/github-search-app.git
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

## Contributing

Feel free to fork this repository and submit pull requests.

---

## License

This project is licensed under the **MIT License**.
