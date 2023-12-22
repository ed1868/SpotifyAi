## Overview
This Python script is a command-line utility for generating and adding playlists to Spotify based on textual prompts. It uses OpenAI's GPT models for playlist suggestion and the Spotipy library for interacting with the Spotify API.

## Features
- Generates playlists based on a given prompt using OpenAI's GPT models.
- Adds the generated playlist to the user's Spotify account.
- Command-line arguments for easy customization of playlist prompt and size.
- Robust error handling and environment variable management.

## Requirements
- Python 3.x
- OpenAI API key
- Spotify Developer credentials (Client ID and Client Secret)
- Spotipy library
- Dotenv for managing environment variables

## Installation
1. Clone the repository.
2. Install required dependencies:
   ```bash
   pip install openai spotipy python-dotenv


Set up a .env file with your OpenAI and Spotify API credentials.
## Usage
Run the script from the command line, providing the necessary arguments:

1. Install required dependencies:
   ```bash
    python script_name.py -p "Your Playlist Prompt" -n [Number of Songs]


## Options:

1. -p: The prompt describing the playlist.
2. -n: The number of songs to be added to the playlist (default is 12).

## Setting Up Spotify Credentials
Register your application at Spotify Developer Dashboard.
Copy your Client ID and Client Secret into your .env file.
Set the redirect URI in your Spotify app settings to http://localhost:9999.

## Functions
main(): Parses command-line arguments and initiates the playlist generation and addition process.
get_playlist(): Generates a playlist based on the given prompt using OpenAI's GPT models.
add_songs_to_spotify(): Adds the generated songs to a new Spotify playlist.
## Error Handling
Checks for the presence of required environment variables.
Validates the number of songs requested.