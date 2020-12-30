# Electron

[Electron | Build cross-platform desktop apps with JavaScript, HTML, and CSS.](https://www.electronjs.org/)

![Electron%20a49b9b9de8ce463c8d5f7991f125d9a6/Untitled.png](Electron%20a49b9b9de8ce463c8d5f7991f125d9a6/Untitled.png)

# Notes:

Getting Started:

1. Create `package.json` file with `npm init` (entry point is `main.js` by convention)
2. Install Electron as dev dependency `npm  i -D electron`
3. Add a start script to package.json "`start": "electron ."`
4. Hack `main.js`(e.g. `import { app, BrowserWindow, Menu } from 'electron'`...
5. `npm run start`

```jsx
function createAboutWindow () {
    aboutWindow = new BrowserWindow({
        title : 'About ImageShrink',
        icon : `${__dirname}/assets/icons/Icon_256x256.png`,
        width : 300,
        height : 300,
        webPreferences: {
            contextIsolation: true
        }
    })
    *aboutWindow.setMenuBarVisibility(false)*
    aboutWindow.loadURL(`file://${__dirname}/app/about.html`)
}
```