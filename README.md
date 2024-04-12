# SOCIAL DOWNLOADER (SOCIAL DL)

![NPM Info](https://nodei.co/npm/social-dl.png?downloads=true&downloadRank=true&stars=true)

[![npm total downloads](https://img.shields.io/npm/dt/social-dl?color=blue)](https://www.npmjs.com/package/social-dl)
[![npm version](https://img.shields.io/npm/v/social-dl?color=blue)](https://www.npmjs.com/package/social-dl)
[![License](https://img.shields.io/npm/l/social-dl?color=blue)](LICENSE)

A simple Node.js tool to generate direct download links for media from **Instagram**, **Facebook**, **Twitter (X)**, **Snapchat**, **TikTok**, and **Pinterest**!  
Just provide the post URL, and this package will return the direct media download URL.

---

## 🚀 Installation

Install via **npm**:

```bash
npm install social-dl
```

Or, if you're using Yarn:

```bash
yarn add social-dl
```

## Usage

### Importing the Package

You can import the entire `social-dl` module:

```javascript
const socialDL = require("social-dl");
```

Or destructure specific functions:

```javascript
const {
  instagramDownloader,
  facebookDownloader,
  twitterDownloader,
  snapchatDownloader,
  tiktokDownloader,
  pinterestDownloader,
} = require("social-dl");
```

### Example Usage

#### Instagram Downloader

```javascript
async function fetchInstagramData() {
  try {
    const result = await socialDL.instagramDownloader(
      "https://www.instagram.com/example-url"
    );
    console.log("Fetched Instagram media details:", result);
  } catch (error) {
    console.error("Error fetching Instagram media details:", error);
  }
}

fetchInstagramData();
```

#### Facebook Downloader

```javascript
async function fetchFacebookData() {
  try {
    const result = await socialDL.facebookDownloader(
      "https://www.facebook.com/example-url"
    );
    console.log("Fetched Facebook media details:", result);
  } catch (error) {
    console.error("Error fetching Facebook media details:", error);
  }
}

fetchFacebookData();
```

#### Twitter Downloader

```javascript
async function fetchTwitterData() {
  try {
    const result = await socialDL.twitterDownloader(
      "https://x.com/example-url"
    );
    console.log("Fetched Twitter media details:", result);
  } catch (error) {
    console.error("Error fetching Twitter media details:", error);
  }
}

fetchTwitterData();
```

#### Snapchat Downloader

```javascript
async function fetchSnapchatData() {
  try {
    const result = await socialDL.snapchatDownloader(
      "https://snapchat.com/example-url"
    );
    console.log("Fetched Snapchat media details:", result);
  } catch (error) {
    console.error("Error fetching Snapchat media details:", error);
  }
}

fetchSnapchatData();
```

#### TikTok Downloader

```javascript
async function fetchTiktokData() {
  try {
    const result = await socialDL.tiktokDownloader(
      "https://www.tiktok.com/example-url"
    );
    console.log("Fetched TikTok media details:", result);
  } catch (error) {
    console.error("Error fetching TikTok media details:", error);
  }
}

fetchTiktokData();
```

#### Pinterest Downloader

```javascript
async function fetchPinterestData() {
  try {
    const result = await socialDL.pinterestDownloader(
      "https://in.pinterest.com/example-url"
    );
    console.log("Fetched Pinterest media details:", result);
  } catch (error) {
    console.error("Error fetching Pinterest media details:", error);
  }
}

fetchPinterestData();
```

## Supported Platforms

- Instagram
- Facebook
- Twitter
- Snapchat
- TikTok
- Pinterest

## Contributing

Contributions are welcome! If you find any issues or want to contribute new features, feel free to fork the repository and create a pull request.

### Steps to Contribute:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature-branch`).
3. Make your changes and commit them (`git commit -am 'Add new feature'`).
4. Push to the branch (`git push origin feature-branch`).
5. Create a pull request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
