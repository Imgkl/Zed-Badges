# Zed-Badges

Welcome to the Zed Extension Badges Workflow repository! This project aims to help Zed extension creators showcase the popularity and current version of their extensions through dynamic badges on their GitHub READMEs. Badges serve as a quick visual reference for potential users, indicating your extension's reliability, usage, and updates.

## Why Use Badges?
- <b>Visibility</b>: Badges make your extension more visually appealing and informative at a glance.
- <b>Credibility</b>: Showing download counts and the latest version builds trust with potential users.
- <b>Consistency</b>: Using standardized badges helps in maintaining a professional look across extension repositories

## How It Works
The workflow automatically fetches the latest download count and version number for your extension from Zed's API and updates the badges in your README.md file. This process runs on a schedule or can be triggered manually, ensuring your badges always reflect the most current data.


## Adding the Workflow to Your Project

Follow these steps to integrate the badge automation into your Zed extension repository:

### Step 1: Prepare Your README.md
Insert placeholders in your README.md where the badges should appear:

```

<!-- BADGES_START -->
<!-- BUILD_FOR_ZED_START -->
<!-- BUILD_FOR_ZED_END -->
<!-- DOWNLOADS_BADGE_START -->
<!-- DOWNLOADS_BADGE_END -->
<!-- VERSION_BADGE_START -->
<!-- VERSION_BADGE_END -->
<!-- BADGES_END -->

```

### Step 2: Add the Workflow File
 - In your repository, navigate to the `.github/workflows` directory. If it doesn't exist, create it.
 - Create a new file named `update-badges.yml`.
 - Copy the contents of the `update-badges.yml` from this repository into your new file.

 The provided workflow performs the following actions:
 - <b>Fetches the latest download count and version number</b> for your extension from the ZED API.
 - <b>Updates the badges</b> in your README.md to reflect the current download count, version number, and a badge indicating it's built for ZED.
- <b>Commits and pushes the changes</b> to your repository automatically, ensuring your badges are always up-to-date.

Once the workflow it's successfully completed, the badges should be added automatically on your readme.

![Badges](https://i.ibb.co/zFxytwL/Screenshot-2024-02-28-at-1-48-30-AM.png)


## Customization
You can customize the workflow to fit your specific needs. For example, you can modify the badge styles or the information they display. Refer to the [Shields.io](Shields.io) documentation for more details on badge customization.


## License
Distributed under the MIT License. See LICENSE for more information.

## Support
If you find this workflow helpful, consider supporting by starring this repository or sharing it with other Zed extension creators!
