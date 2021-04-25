# **TODOS**
## **Set up the Chrome Extension App**
### Create file `"manifest.json"`:
- Extensions start with their `manifest`. Create a file called `manifest.json` and include the following code.
```
{
    "name": "Rocket Planner",
    "description": "MOST EPIC EVER",
    "version": "1.0"
}
```
1. Open the Extension Management page by navigating to `chrome://extensions`.
    - Alternatively, open this page by clicking on the Extensions menu button and selecting `Manage Extensions` at the bottom of the menu.
    - Alternatively, open this page by clicking on the Chrome menu, hovering over `More Tools` then selecting `Extensions`
2. Enable `Developer Mode` by clicking the toggle switch next to Developer mode.
3. Click the `Load unpacked button` and select the extension directory.
- Add icons for the extensions:
```
{
    "name": "The Rocket Planner",
    "description": "MOST EPIC EVER",
    "version": "1.0",
    "browser_action": {
        "default_popup": "popup.html",
        "default_icon": {
            "16": "images/icons16.png",
            "32": "images/icons32.png",
            "48": "images/icons48.png",
            "128": "images/icons128.png"
        }
    },
    "icons": {
        "16": "images/icons16.png",
        "32": "images/icons32.png",
        "48": "images/icons48.png",
        "128": "images/icons128.png"
    },
    "manifest_version": 2
}
```
- Create `popup.html`
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    <h1>Hello World</h1>
</body>
</html>
```