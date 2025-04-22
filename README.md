<div align="center"> 

<h3>📱 A modern job search app built with React Native and Expo</h3> </div>
📌 Table of Contents
📖 Overview

⚙️ Tech Stack

✨ Features

🚀 Getting Started

🖼️ Snippets

📎 Resources

🙌 Contributing

📖 Overview
HireHub is a feature-rich React Native application designed to help users find jobs with ease. Whether you're exploring nearby opportunities or searching for specific job titles, HireHub has you covered with a responsive UI and seamless API integration.

Watch the full tutorial and learn to build this app on JavaScript Mastery YouTube

⚙️ Tech Stack
React Native (Expo)

Node.js

Axios

RapidAPI - JSearch

Custom React Hooks

Expo Router & Navigation

✨ Features
✅ Beautiful & Responsive UI
✅ Browse Jobs by Category or Location
✅ Search with Pagination
✅ Custom API Integration via RapidAPI
✅ Detailed Job Descriptions
✅ Reusable Components & Hooks
✅ Error Handling & Loaders
✅ Optimized for Mobile Devices

🚀 Getting Started
Prerequisites
Make sure you have the following installed:

Node.js

Expo CLI

Git

RapidAPI account

Installation Steps
bash
Copy code
# Clone the repository
git clone https://github.com/your-username/hirehub.git
cd hirehub

# Install dependencies
npm install
Setup Environment
Create a .env file in the root directory and add your RapidAPI key:

env
Copy code
X-RapidAPI-Key=your_key_here
Run the App
bash
Copy code
npm start
Scan the QR code with Expo Go to view the app on your device.

🖼️ Snippets
<details> <summary><code>Search.js</code></summary>
js
Copy code
useEffect(() => {
  const fetchJobs = async () => {
    setSearchLoader(true);
    try {
      const response = await axios.get("https://jsearch.p.rapidapi.com/search", {
        params: { query: params.id, page: page },
        headers: {
          "X-RapidAPI-Key": process.env.X_RAPIDAPI_KEY,
          "X-RapidAPI-Host": "jsearch.p.rapidapi.com"
        }
      });
      setSearchResult(response.data.data);
    } catch (error) {
      setSearchError(true);
    } finally {
      setSearchLoader(false);
    }
  };
  fetchJobs();
}, [page]);
</details>