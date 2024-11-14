## Features

- **Explore**: Retrieve a curated list of anime from the home page, excluding specific categories for a cleaner view.
- **Search**: Search feature to find anime by title or keywords.
- **Anime Info**: Get comprehensive details about a specific anime, including seasons and other related data.
- **Basic Anime Info**: Access essential information about an anime, stripped of unnecessary details, allowing for quick reference.
- **Episode List**: Fetch a list of episodes for a given anime, with caching to minimize repeated data retrieval and to optimize loading times.
- **Episode Servers**: Retrieve server names for streaming episodes.
- **Server Video Sources**: Get sources for streaming episodes from a specific server, including additional metadata like subtitles.
- **Caching**: Utilize Redis for caching responses to minimize database hits and improve application speed, with varying expiration times based on data type.