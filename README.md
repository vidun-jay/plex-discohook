## Overview
Plex Webhook Server is a Node.js application designed to interact with Plex media server URLs. It allows users to submit a URL from the Plex platform and specifies the media library category (e.g., Anime, Movies, TV Shows). The server processes these URLs using Puppeteer to scrape relevant media information, then sends a formatted message to a specified Discord webhook, notifying about media additions to Plex libraries.

## Installation
Instructions on how to install and set up the project will be added here.

## Creating a Discord Webhook
To use the Discord integration feature, you need to create a webhook in your Discord server. Here’s how to set it up:

1. Open Discord: Go to your server where you have the necessary permissions.
2. Server Settings: Click on the server name, then select Server Settings.
3. Integrations: Go to the Integrations tab and click on Webhooks.
4. New Webhook: Click on New Webhook. Name your webhook and choose the channel where messages will be posted.
5. Copy Webhook URL: After creating the webhook, click the Copy Webhook URL button to get the URL. This is the URL you will use in your project to send messages to Discord.

## How to Use
1. Start the Server: Run the server using Docker or directly with Node.js (details will be provided in the Installation section).
2. Access the Web Interface: Open your web browser and navigate to http://localhost:3000. This will load the interactive interface.
3. Enter Plex URL: In the web interface, input a valid Plex URL into the URL field.
4. Select Library: Choose the appropriate library category for the media from the dropdown menu.
5. Submit: Click the submit button. If the URL is valid and the server is able to process it, the details of the media will be scraped and sent to the specified Discord channel.
6. Discord Notification: Check the configured Discord channel for the notification that includes the title, description, and other relevant details of the media added to Plex.

## Local Development
### Prerequisites
Node.js (v14 or above)
Docker (for containerization)
Access to a Discord server and permissions to manage webhooks

### Running Locally
To run the server locally without Docker, follow these steps:

Install dependencies: `npm install`
Start the server: `node server.js`
Visit http://localhost:3000 in your browser to use the application.
