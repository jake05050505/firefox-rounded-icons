# firefox-rounded-icons

## Setup

>### 1. Allow stylesheets to be rendered by firefox
> - type `about:config`, Click Accept if prompted.
> - find `toolkit.legacyUserProfileCustomizations.stylesheets` using the searchbox.
> - toggle the setting above either by double clicking it, or clicking the toggle button to its right.

>### 2. Finding your firefox profile folder
> - type `about:support` into your address bar. Alternatively, you can enter `about:profiles`.
> - If using `about:support`, look for the heading "Application Basics", scroll down until you see the field "Profile Folder". Click the "Open Folder" button.
> - If using `about:profiles`, find your default profile (`Default Profile: yes`), find the Root Directory field and click "Open Folder".

>### 3. Setting up userChrome.css
> - After step 2, your default file explorer should open to `Firefox/Profiles/___.default-release-___`
> - In this directory, create a new folder called `chrome`.
> - Enter the new folder.
> - Now you can either copy the [`userChrome.css`](https://github.com/jake05050505/firefox-rounded-icons/blob/main/userChrome.css) file from this repository, or create a new file in `chrome/` called `userChrome.css`, and copy/paste the contents of the [`userChrome.css`](userChrome.css) file from this repository (The same code can also be found below).

```
#back-button > .toolbarbutton-icon,
#forward-button > .toolbarbutton-icon,
#reload-button > .toolbarbutton-icon,
#stop-button > .toolbarbutton-icon,

.toolbarbutton-badge-stack,
.identity-box-button,
#tracking-protection-icon-container,
#urlbar-searchmode-switcher {
    border-radius: 9999px !important;
}

.button-background {
    border-radius: 9999px !important;
}

.tab-background,
#tabs-newtab-button {
    border-radius: 20px !important;
}

#unified-extensions-button > .toolbarbutton-icon {
    border-radius: 11px !important;
}

.urlbar-background {
    border-radius: 20px !important;
}

.urlbar-page-action {
    visibility: hidden !important;
}
```
