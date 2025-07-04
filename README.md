# TheTracker Auth Pages

This repository contains authentication-related web pages for TheTracker iOS app.

## Purpose

This repository hosts the password reset page that handles authentication redirects from Supabase. When users request a password reset in the TheTracker app, they receive an email with a link to this page, which then securely redirects them back to the app with the necessary authentication tokens.

## How It Works

1. User requests a password reset in the TheTracker app
2. Supabase sends an email with a reset link to this page
3. This page extracts the authentication tokens and redirects back to the app using a custom URL scheme
4. The app handles the reset process with the tokens

## Development

This is a simple static HTML page hosted on GitHub Pages. No build process is required.

## Privacy

This page does not collect any user data. It only serves as a bridge between Supabase authentication and the TheTracker app. 