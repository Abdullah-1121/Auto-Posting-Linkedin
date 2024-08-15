# Auto-Posting-Linkedin
# Post on LinkedIn - Custom GPT Automation

This project automates posting on LinkedIn using a custom GPT named "Post on LinkedIn" through Zapier webhooks. The custom GPT requires a title, body, and image URL for the post, and Zapier handles the automation of posting it to LinkedIn.

## Overview

This project allows you to automate the process of posting content on LinkedIn by providing:
- **Title** of the LinkedIn post
- **Body** text for the post
- **Image URL** that will be attached to the post

The workflow is built using Zapier and integrates with a custom GPT that processes the input data and posts it on LinkedIn.

## Features

- Automated LinkedIn posts using a custom GPT.
- Integration with Zapier for seamless automation.
- Customizable post content including title, body, and image.

## Prerequisites

- **Zapier Account**: To create and manage the Zap for automation.
- **Custom GPT**: You need to have a custom GPT created for handling LinkedIn posts.
- **LinkedIn Account**: To authenticate and post content.

## Setup

### 1. Setup Zapier Webhook

- Create a new Zap in Zapier.
- Set up a trigger using **Webhooks by Zapier**.
- Configure the trigger to receive data from your custom GPT.

### 2. Custom GPT Setup

Ensure your custom GPT is configured to accept the following inputs:

- **Title**: The title of the LinkedIn post.
- **Body**: The main content of the LinkedIn post.
- **Image URL**: The URL of the image to be included in the post.

### 3. Connect LinkedIn to Zapier

- Add LinkedIn as the action app in your Zap.
- Set up the action to create a new post with the data provided by the webhook (Title, Body, Image URL).

## Usage

### 1. Trigger the Post

Send a request to the Zapier webhook URL with the required data:

```json
{
  "title": "Your Post Title",
  "body": "The content of your LinkedIn post.",
  "image_url": "https://example.com/your-image.jpg"
}
