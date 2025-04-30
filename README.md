# **Elite Dangerous Ease \- Help Document**

**Elite Dangerous Ease** is a powerful WPF overlay tool designed to enhance your Elite Dangerous experience, with optional VR support for immersive gameplay. It streamlines tasks like managing blueprints, tracking colonization projects, and accessing game information, and is fully functional in desktop mode. VR (optional) uses SteamVR or Desktop+ (recommended) to display interactive overlay windows, controllable via HOTAS, keyboard, or mouse. The app takes focus from the game for navigation and returns focus when hidden, ensuring a seamless experience in both desktop and VR (optional) modes.

**Important**: This application is not affiliated with, endorsed by, or sponsored by Frontier Developments, the developers of Elite Dangerous. All Elite Dangerous terminology (e.g., "journal files," "systems," "blueprints," "market data") is the intellectual property of Frontier Developments and is used for compatibility.

## **Table of Contents**

* Overview  
* Prerequisites  
* Installation  
* Configuration  
* UI Navigation  
* Main Sections  
  * Home  
  * Find  
  * Engineering  
  * Colonization  
  * Macro  
* Support the Project  
* License  
* Troubleshooting

## **Overview**

Elite Dangerous Ease enhances Elite Dangerous gameplay in desktop mode, with optional VR support for users with VR headsets. In VR (optional), overlay windows (e.g., commander status, blueprints) are managed by SteamVR or Desktop+ (recommended), appearing as interactive panels in your headset. The app supports HOTAS controllers for intuitive navigation and takes focus from the game for interaction, returning focus when hidden. Key features include:

* Journal file processing for real-time data (e.g., market info, commander status).  
* Navigation with HOTAS (e.g., POV, Button1), keyboard (WASD), or mouse.  
* Blueprint management, colonization tracking, and macro execution.  
* Discord integration for sharing logs and documentation.  
* Plot Route with specific key bindings.

The app also runs smoothly in desktop mode.

## **Prerequisites**

* **Elite Dangerous**: Installed, with journal files in %USERPROFILE%\\Saved Games\\Frontier Developments\\Elite Dangerous (e.g., Journal.2025-04-29T123456.01.log).  
* **Graphics Mode**: Set to **BORDERLESS** for optimal overlay performance (required for desktop).  
* **VR Setup (Optional)**:  
  * Compatible with VR headsets (e.g., Oculus, Vive, Valve Index) if VR is desired.  
  * Configure Elite Dangerous for VR mode (optional).  
  * Install a VR overlay system (required only for VR):  
    * **SteamVR**: Included with SteamVR-compatible headsets. Ensure SteamVR is running.  
    * **Desktop+** (recommended): Download from Desktop+ GitHub or Steam for better performance.  
* **HOTAS/Controller**: Optional, but works for both desktop and VR. Map buttons (e.g., Button10 for toggle, POV for navigation) in Elite Dangerous or the app.  
* **System Requirements**: Windows with .NET Framework 4.8 or .NET 6+.  
* **Google Drive API**: Required for **COLONIZATION** (free; see Configuration).  
* **Key Bindings**: Specific bindings for **Plot Route** (see Configuration).

## **Installation**

1. **Download**: Get the [Latest Release](https://github.com/shalkecsharp/EDE/releases/latest)
2. **Unzip**: Extract ede.zip to any folder (e.g., C:\\Games\\EliteDangerousEase).  
3. **Set Up VR Overlay System (Optional)**:  
   * If using VR, configure a VR overlay system:  
     * **SteamVR**: Launch SteamVR, enable overlay support (SteamVR Settings \> General).  
     * **Desktop+** (recommended): Install from Desktop+ GitHub or Steam. Add EliteDangerousEase.exe as a VR overlay (see Desktop+ documentation).  
   * Skip this step for desktop mode.  
4. **Run**: Double-click EliteDangerousEase.exe.  
5. **First Launch**:  
   * Processes journal files, generating logs in the logs folder (e.g., ede\_2025-04-29.log). This may take a few minutes.  
   * In VR (optional), overlays appear via SteamVR or Desktop+; adjust position/opacity in their settings.  
6. **Verify**:  
   * Toggle with **Right CTRL** (keyboard) or **Button10** (HOTAS).  
   * Ensure panels (e.g., HOME, FIND) are visible in desktop or VR (if enabled).

**Note**: VR is optional. The app works fully in desktop mode. For VR, use Desktop+ for optimal overlay performance or SteamVR for standard support. Adjust VR overlay positions if needed.

## **Configuration**

* **Colonization**:  
  * Requires Google Drive API (free).  
  * **Steps**:  
    * Go to Google Cloud Console.  
    * Create a project, enable Google Drive API.  
    * Generate OAuth 2.0 credentials (client ID, secret).  
    * Download credentials JSON to app directory (e.g., credentials.json).  
    * Authenticate via **COLONIZATION \> SETTINGS**.  
  * See Google Drive API Docs.  
* **Plot Route**:  
  * Set Elite Dangerous key bindings:  
    * Open galaxy map: **O**  
    * UI up: **W**  
    * UI down: **S**  
    * UI select: **SPACE**  
    * Galaxy map zoom: **Z**  
  * Remove **W** and **S** from General \> Galaxy Map controls.  
* **VR Overlay System (Optional)**:  
  * If using VR:  
    * **SteamVR**: Enable overlays (SteamVR Settings \> General).  
    * **Desktop+**: Add EliteDangerousEase.exe as an overlay (Dashboard \> Add Application). Adjust opacity/size/position.

## **UI Navigation**

The overlay takes focus from Elite Dangerous for navigation and returns focus when hidden. In VR (optional), overlays are managed by SteamVR or Desktop+ (recommended). Navigate with keyboard, mouse, or HOTAS.

* **Toggle**:  
  * **Keyboard**: **Right CTRL**.  
  * **HOTAS**: **Button10**.  
* **Keyboard**:  
  * **Q, E**: Switch tabs (e.g., HOME, FIND).  
  * **W, A, S, D**: Navigate panels/UI elements.  
  * **SPACE**: Trigger actions (e.g., select, pin blueprints).  
  * **BACKSPACE**: Return to parent panel.  
* **Mouse**:  
  * Click buttons/items.  
  * Note: **Plot Route** not yet mouse-supported.  
* **HOTAS/Controller**:  
  * **Button3, Button4**: Switch tabs.  
  * **POV**: Navigate panels.  
  * **Button1**: Actions.  
  * **Button2**: Back.  
* **Navigation Notes**:  
  * In desktop mode: Use a 30px drag handle to reposition.  
  * In VR (optional): Overlays appear via SteamVR or Desktop+ (recommended for smoother performance). Navigate with HOTAS POV/Button1 or keyboard. The app takes focus when shown, returns focus to game when hidden.  
* **VR Note (Optional)**: If using VR, configure SteamVR or Desktop+ for overlay visibility. Desktop+ offers customizable positioning.

Header buttons: **HOME**, **FIND**, **ENGINEERING**, **POWER PLAY**, **COLONIZATION**, **MACRO**

## **Main Sections**

Panels are accessible via tabs.

### **Home**

Displays messages and status.

* **STATUS**:  
  * Shows commander status (credits, rank), location, merits.

### **Find**

Search for systems, stations, resources.

* **RECENT LOCATIONS**:  
  * Lists visited stations/planets from journal files.  
  * Select with **SPACE** (Button1) for details or **Plot Route**.  
* **NEAREST**:  
  * Finds material traders/manufactured materials.  
* **NEUTRON PLOTTER**:  
  * Shows next jump from imported Neutron Plotter plot.  
  * Select with **SPACE** (Button1).  
* **INARA**:  
  * Links to Inara for system/commander data.

### **Engineering**

Manages blueprints, engineers, ships.

* **BLUEPRINTS**:  
  * Browse/pin blueprints with **WASD** (POV), **SPACE** (Button1).  
* **ENGINEERS**:  
  * Shows engineer details.  
* **SHIPS**:  
  * Lists ships/modules.  
  * **SPACE** (Button1) for **Plot Route**.

### **Colonization**

Manages colonization projects (Google Drive API).

* **COLONIZATION PROJECTS**:  
  * Displays project data (progress, resources).  
* **ADD PROJECT**:  
  * Creates project from a docked construction site data.  
* **SETTINGS**:  
  * Configures Google Drive, overlay visibility, projects.  
* **Note**: In VR (optional), project overlays are adjustable via Desktop+.

### **Macro**

Configures keystroke macros.

* **PATTERN 1**:  
  * Manages macro script (keys, timing).  
  * Assign shortcut or HOTAS button.

## **License**

Proprietary license (see LICENSE.txt). Key points:

* Free for personal, non-commercial use.  
* No modification/reverse-engineering/redistribution.  
* Not affiliated with Frontier Developments; Elite Dangerous terminology is their property.  
* View via **LICENSE** button.

## **Troubleshooting**

Use **POST LOG** button left of Close button in the top right corner. Feel free to ask on [Discord](https://discord.gg/NY688QpZ)
