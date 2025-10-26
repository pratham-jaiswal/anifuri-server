![](https://i.imgur.com/wIANk1D.png)

# Anifuri Server

Anifuri is a open-source free anime streaming application designed to provide you with an easy and simple way to discover, watch, and enjoy your favorite anime. With a wide range of features, Anifuri allows users to explore trending titles, keep track of episodes, and easily search for anime. Whether you're looking for the latest episodes or want to revisit classic favorites, Anifuri offers a seamless streaming experience tailored to your needs.

> <h2 align="center">DISCLAIMER</h2>
> <p align="center"><i>Anifuri does not host or store any anime content. All data fetched and displayed within the app is sourced from external platforms. We provide a service that allows users to stream anime, but we do not keep any of the streams or content on our end. Please ensure you are in compliance with local laws regarding streaming content.</i></p>

## Project Discontinued - But You Can Still Run It Yourself

This project is no longer actively maintained.
However, you can still **set it up, host it, or build upon it** on your own using the steps below.

[App Repository](https://github.com/pratham-jaiswal/anifuri)

### ⚙️ Setup Steps

1. **Fork or Clone the repo**

   * **If you plan to contribute or modify the project**, fork it to your own GitHub account by clicking on the fork button on top of the repo or clicking on this [link](https://github.com/pratham-jaiswal/anifuri-server/fork), then

    ```bash
    git clone https://github.com/<your-username>/anifuri-server.git
    cd anifuri-server
    ```

    * **If you just want to use or run the app**, clone it directly:

    ```bash
    git clone https://github.com/pratham-jaiswal/anifuri-server.git
    cd anifuri-server
    ```

2. **Install dependencies:**

    ```bash
    npm install
    ```

3. **Create a `.env` file** in the project root with the following:

    ```env
    REDIS_URL=redis://localhost
    REDIS_PORT=6379
    REDIS_PASSWORD=redis_password
    ```

    > You can either:
    > * **Run Redis locally** using Docker or your system package manager, or
    > * **Use a free hosted Redis** instance (e.g., [Upstash](https://upstash.com) or [Redis Cloud](https://redis.io/try-free/)) and replace the URL, port, and password accordingly.

4. [Deploy](#-to-deploy) or [Run](#-to-run-locally)

### 📱 To Deploy

5. Deploy as a **serverless function on [Vercel](https://vercel.com)** *(free)* or host it on **Heroku**, **DigitalOcean**, etc. for paid, persistent setups.
    > Don't forget to configure and import your environment variables on your hosted server.

### 💻 To Run Locally

5. **Start the server**

    ```bash
    npm start
    ```

    or (for live reload during development)

    ```bash
    nodemon
    ```

## Features

- **Search Anime**: Search for your favorite anime.
- **Explore Anime**
  - **Spotlight Anime**: Highlighted anime recommendations based on trends.
  - **Continue Watching**: Easily access anime you have started but not finished.
  - **Trending Anime**: Explore the currently trending anime.
  - **Latest Episodes**: Stay updated with the latest episodes of your favorite series.
  - **Top Airing Anime**: Discover top anime that are currently being released.
  - **Most Popular Anime**: Find the most popular anime.
  - **Most Favorite Anime**: Discover anime that are highly rated and loved by the community.
  - **Latest Completed Anime**: Find anime that have recently finished airing.
- **Anime Details**: Display detailed information about a specific anime.
- **Episodes List**: View a list of episodes.
- **Stream with Subtitles**: Stream episodes with subtitles.
- **Server Selection**: Choose different servers for episodes to stream them.
- **Mark as Watched**: Mark any _finished airing_ anime as watched.
- **Watched Anime**: View a list of your watched anime.
- **Clear History**: Clear the watched and currently watching anime data.

## Built With

- [Express.js](https://expressjs.com/)
- [AniWatch](https://github.com/ghoshRitesh12/aniwatch)
