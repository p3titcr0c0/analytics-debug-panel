#  ![icon](./static/icons/48.png) Analytics Debug Panel

> Chrome, Firefox & Opera Browser Extension - Analytics Debug Panel

#  ![demo](./demo.gif)

[Red Van Workshop](https://redvanworkshop.com) works with online retailers that have a variety of Analytic Providers for their differing business needs.  Working on new integrations and debugging existing ones is an integral part of our developer process.  This Browser Extension was built to help make that process easier.  We hope you will find it as useful as we do, and if you want to help make it better, we'd love to hear from you.

## Installation

> Here is how to install this extension in your favorite browsers:

<details><summary>Add to Google Chrome</summary>

1. Download [Webkit Extension](https://github.com/redvanworkshop/analytics-debug-panel/raw/master/dist/webkit-extension.crx)
2. Click **Keep** when prompted to download the file
3. Go to the following URL in a new Google Chrome tab:  `chrome://extensions/`
4. In the top right corner, Enable **Developer Mode**
5. Drag and Drop `webkit-extension.crx` file into Extension page

</details>

<details><summary>Add to Firefox</summary>

1. Download [Webkit Extension](https://github.com/redvanworkshop/analytics-debug-panel/raw/master/dist/firefox-addon.zip)
2. Open Firefox
3. Go to the following URL in a new tab:  `about:debugging`
4. Select `Enable add-on debugging` checkbox
5. In the top right corner, Click **Load Temporary Add-on**
6. Select the `firefox.zip` file

</details>

<details><summary>Add to Opera</summary>

1. Download [Webkit Extension](https://github.com/redvanworkshop/analytics-debug-panel/raw/master/dist/webkit-extension.crx)
2. Go to the following URL in a new Opera tab:  `chrome://extensions/`
3. In the top right corner, Enable **Developer Mode**
4. Drag and Drop `webkit-extension.crx` file into Extension page
5. Select **Yes, Install** when prompted

</details>

## Developers

<details><summary>Support New Providers</summary>

> Adding New Analytics Providers is Easy

1. Create a new folder in `./src/providers` following the standard we have in place
2. Create a new `index.js` file inside that new folder
3. See `./src/providers/google-universal-analytics/index.js` for an example
4. Submit a PR for use to review the new Providers
5. High Five on a Job Well Done

</details>

<details><summary>Build Extension</summary>

```bash
git clone git@github.com:redvanworkshop/analytics-debug-panel.git
cd analytics-debug-panel
npm install
npm run build
```

</details>

<details><summary>Load Unpacked Extension to Google Chrome</summary>

1. Open Google Chrome
2. Go to the following URL in a new tab:  `chrome://extensions/`
3. In the top right corner, Enable **Developer Mode**
4. Click the **LOAD UNPACKED** link in the header
5. Select the `./analytics-debug-panel/build` folder

</details>

<details><summary>Load Temporary Add-on to Firefox</summary>

1. Open Terminal in project root and run `npm run pack:firefox`
2. Open Firefox
3. Go to the following URL in a new tab:  `about:debugging`
4. Select `Enable add-on debugging` checkbox
5. In the top right corner, Click **Load Temporary Add-on**
6. Select the `firefox.zip` file

</details>

<details><summary>Load Unpacked Extension to Opera</summary>

1. Open Opera
2. Go to the following URL in a new tab:  `chrome://extensions/`
3. In the top right corner, Enable **Developer Mode**
4. Drag and Drop `./analytics-debug-panel/build` folder into Extension page

</details>

<details><summary>Pack Extensions</summary>

```bash
cd analytics-debug-panel
npm run pack
```

</details>
