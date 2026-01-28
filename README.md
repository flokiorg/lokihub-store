# How to Submit an App to Lokihub

App registry and discovery for the Lokihub ecosystem. This list is community-driven, and we welcome submissions from developers.

## How it works

The list of apps is stored in `apps.json`. To add your app, you need to fork this repository, add your app's details to the JSON file, and open a Pull Request (PR).

## Submission Steps

1.  **Fork the Repository**: Create a fork of the `lokihub` repository.
2.  **Add App Logo**:
    *   Place a high-quality logo of your app in the `logos` directory.
    *   The logo should be a PNG or SVG file.
    *   Recommended size: 512x512 pixels.
    *   Name the file `your-app-id.png` (e.g., `my-awesome-app.png`).
3.  **Edit `apps.json`**:
    *   Add a new object to the array with your app's details.
    *   Please maintain the alphabetical order (or append to the end, and we will sort it).
4.  **Create a Pull Request**: Submit your changes for review.

## JSON Schema

Here is the structure of an app entry:

```json
{
  "id": "my-app",
  "title": "My App",
  "description": "Short description of your app (max 100 chars)",
  "extendedDescription": "Longer description explaining the integration with Lokihub/Flokicoin",
  "webLink": "https://myapp.com",
  "playLink": "https://play.google.com/store/apps/details?id=com.myapp",
  "appleLink": "https://apps.apple.com/us/app/my-app/id123456",
  "category": "social-media",
  "logo": "my-app.png",
  "installGuide": "Instructions for installing the app",
  "finalizeGuide": "Instructions for connecting the app to Lokihub",
  "version": "1.0.0",
  "createdAt": 1700000000,
  "updatedAt": 1700000000
}
```

### Fields

*   `id` (Required): A unique identifier for your app (lowercase, dashes only).
*   `title` (Required): The display name of your app.
*   `description` (Required): A short tagline.
*   `extendedDescription`: A more detailed explanation.
*   `webLink`: URL to your app's website.
*   `playLink`: URL to the Google Play Store.
*   `appleLink`: URL to the Apple App Store.
*   `category`: The category of the app. Allowed values:
    *   `wallet-interfaces`
    *   `social-media`
    *   `ai`
    *   `merchant-tools`
    *   `music`
    *   `blogging`
    *   `payment-tools`
    *   `shopping`
    *   `nostr-tools`
    *   `games`
    *   `misc`
*   `logo`: Filename of the logo in `logos/` (must be PNG).
*   `installGuide`: Text describing how to install/setup the app before connection.
*   `finalizeGuide`: Text describing the connection process (e.g. where to paste the secret).
*   `version` (Required): Semantic version of the app (e.g., "1.0.0").
*   `createdAt` (Required): Unix timestamp of creation.
*   `updatedAt` (Required): Unix timestamp of last update.

## Review Process

Once you submit your PR, the Lokihub maintainers will review your submission. We check for:
*   Valid JSON format.
*   Appropriate content and categorization.
*   Working links.
*   High-quality logo.

Thank you for contributing to the Flokicoin ecosystem!
