# chrome-extension-tutorials

The Chrome Extension API provides a wide range of functionalities for developing extensions. Here's a list of some of the main APIs available for Chrome extensions:

1. **chrome.runtime**: Provides information about the Chrome extension runtime environment and enables communication between different parts of the extension.
2. **chrome.tabs**: Allows manipulation of browser tabs and their properties.
3. **chrome.windows**: Provides functions to manipulate browser windows and their properties.
4. **chrome.bookmarks**: Enables interaction with the user's bookmarks and bookmark folders.
5. **chrome.browserAction**: Allows manipulation of the browser toolbar icon and associated popup.
6. **chrome.contextMenus**: Allows adding items to the browser's context menu.
7. **chrome.commands**: Enables registering keyboard shortcuts for the extension.
8. **chrome.notifications**: Allows the extension to create and manage desktop notifications.
9. **chrome.storage**: Provides access to local and sync storage areas for storing extension data.
10. **chrome.cookies**: Allows manipulation of cookies for the current website.
11. **chrome.identity**: Enables OAuth2 authentication and user identity management.
12. **chrome.webRequest**: Allows monitoring, blocking, and modifying HTTP requests.
13. **chrome.webNavigation**: Provides information about the navigation events in the browser.
14. **chrome.webRequestBlocking**: Allows synchronous blocking of HTTP requests.
15. **chrome.runtime.connect**: Enables communication between different parts of the extension using message passing.
16. **chrome.runtime.onInstalled**: Event fired when the extension is installed, updated, or enabled.
17. **chrome.runtime.onMessage**: Event fired when a message is sent from another part of the extension or a content script.
18. **chrome.runtime.onConnect**: Event fired when a connection is made from another part of the extension.
19. **chrome.i18n**: Provides internationalization features for the extension, including message localization.
20. **chrome.permissions**: Allows the extension to request additional permissions dynamically.
21. **chrome.windows.onFocusChanged**: Event fired when the focus changes from one window to another.

These are some of the main APIs provided by the Chrome Extension platform. There are additional APIs and events available for specific functionalities and permissions required by extensions. Always refer to the official Chrome Extension documentation for the most accurate and detailed information about each API.


As of my last update in January 2022, the `chrome.runtime` namespace in Chrome extensions provides several functions and properties for interacting with the extension runtime environment. Here are some of the commonly used functions and properties available in `chrome.runtime`:

1. **Methods**:
   - `sendMessage`: Sends a single message to an extension or a different extension.
   - `connect`: Connects to a native application.
   - `getBackgroundPage`: Gets the background page for the extension.
   - `getManifest`: Retrieves the extension's manifest file.
   - `getURL`: Converts a relative path within an extension install directory to a full URL.
   - `reload`: Reloads the extension.
   - `requestUpdateCheck`: Requests an update check for this extension.
   - `restart`: Restarts the Chrome browser and optionally relaunches the extension.
   - `sendNativeMessage`: Sends a single message to a native application.
   - `setUninstallURL`: Sets the URL to be visited upon uninstallation of the extension.
   - `getPlatformInfo`: Retrieves information about the platform the extension is running on.
   - `getPackageDirectoryEntry`: Gets the DirectoryEntry for the package directory.

2. **Events**:
   - `onInstalled`: Fired when the extension is first installed, when the extension is updated to a new version, and when Chrome is updated to a new version.
   - `onMessage`: Fired when a message is sent from either an extension process (by `runtime.sendMessage`) or a content script (by `tabs.sendMessage`).
   - `onConnect`: Fired when a connection is made from either an extension process or a content script.
   - `onConnectExternal`: Fired when a connection is made from another extension.
   - `onStartup`: Fired when Chrome is launched.

These are some of the essential methods and events provided by `chrome.runtime`. There might be additional methods and events available depending on the Chrome version and the features supported by the extension platform. Always refer to the latest Chrome extension documentation for the most accurate and up-to-date information.



The `chrome.tabs` API in Chrome extensions provides a wide range of functionalities for manipulating browser tabs and accessing their properties. Here's a list of some of the main methods, events, and properties available in the `chrome.tabs` API:

### Methods:
1. **`chrome.tabs.create`**: Creates a new browser tab.
2. **`chrome.tabs.update`**: Updates the properties of a specific tab.
3. **`chrome.tabs.get`**: Retrieves details about a specific tab.
4. **`chrome.tabs.getCurrent`**: Retrieves details about the currently active tab in the current window.
5. **`chrome.tabs.query`**: Retrieves details about one or more tabs that match specified criteria.
6. **`chrome.tabs.remove`**: Closes one or more tabs.
7. **`chrome.tabs.duplicate`**: Duplicates a tab.
8. **`chrome.tabs.move`**: Moves one or more tabs to a new position within the current window or to a new window.
9. **`chrome.tabs.reload`**: Reloads a specific tab or multiple tabs.
10. **`chrome.tabs.executeScript`**: Injects JavaScript code into a tab.
11. **`chrome.tabs.insertCSS`**: Injects CSS into a tab.
12. **`chrome.tabs.detectLanguage`**: Detects the language of the content in a tab.

### Events:
1. **`chrome.tabs.onCreated`**: Fired when a new tab is created.
2. **`chrome.tabs.onUpdated`**: Fired when a tab is updated, such as when its URL changes or when the page title changes.
3. **`chrome.tabs.onActivated`**: Fired when the active tab in a window changes.
4. **`chrome.tabs.onRemoved`**: Fired when a tab is closed.
5. **`chrome.tabs.onReplaced`**: Fired when a tab is replaced with another tab due to prerendering or instant.
6. **`chrome.tabs.onMoved`**: Fired when a tab is moved within a window.
7. **`chrome.tabs.onDetached`**: Fired when a tab is detached from a window.
8. **`chrome.tabs.onAttached`**: Fired when a tab is attached to a window.
9. **`chrome.tabs.onHighlighted`**: Fired when the highlighted or selected tabs in a window changes.

### Properties:
1. **`chrome.tabs.Tab`**: Represents a browser tab.
2. **`chrome.tabs.TabStatus`**: Represents the status of a tab, such as 'loading', 'complete', etc.

These are some of the main methods, events, and properties available in the `chrome.tabs` API. They allow developers to interact with and manipulate browser tabs in various ways within Chrome extensions.
