# Ridibooks Chapter Downloader

A custom browser script built to intercept and save high-resolution episode pages from Ridibooks directly to your computer. It monitors background network traffic to grab the original picture links and organizes them into a local directory.

## ✨ Main Features

* **Backend Interception:** Listens for the site's internal `generate` network requests (via Fetch and XHR) to silently capture the raw image array as soon as the page loads.
* **Auto-Recovery System:** If a network timeout occurs, the tool automatically pauses for two seconds and re-attempts the download up to three times per picture.
* **Paced Processing:** Enforces a strict 200-millisecond delay between each file request to ensure your browser remains stable and does not throttle the connection.
* **Interactive Interface:** Injects a dynamic, floating status button in the bottom corner of your screen. It displays a waiting status initially and turns blue once the page data is ready to process.
* **Native Directory Saving:** Automatically sanitizes the book's title to create a valid folder on your hard drive, saving each file sequentially without requiring ZIP extraction.
* **Dynamic Reset:** Instantly clears its cache and resets the user interface when you navigate to a new episode without needing a full page refresh.

## 🚀 Setup and Execution

1. **Requirements:** You must have the **Tampermonkey** extension installed to grant the necessary local file-saving permissions.
2. **Installation:** Add the code through the Greasyfork repository.
3. **Usage:** Open any reading session on Ridibooks. The floating button will initially show a searching status.
4. **Save:** Once the button turns blue and displays the total page count, click it to queue and save all the images to your device.

## ⚠️ Important Notice

**This project is intended strictly for personal archiving and educational study.** Please support the original authors and publishers. Do not upload, share, or redistribute the saved media under any circumstances.

## 🔗 Links and Support

* **Script Library:** [ozler365 on Greasyfork](https://greasyfork.org/en/users/1553223-ozler365)
* **GitHub Portfolio:** [ozler-s-works-info](https://ozler365.github.io/ozler-s-works-info/#/repositories)
* **Support the Developer:** If this tool helps you out, consider leaving a tip at [Buy Me a Coffee (ozler)](https://buymeacoffee.com/ozler).

For bug reports, feature suggestions, or general questions, please drop a review on Greasyfork or send an email to **devjk6918@gmail.com**.
