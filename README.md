**Elite Dangerous Ease**
Elite Dangerous Ease is a tool to help you manage various aspects of Elite Dangerous Game, making it easier to handle blueprints, colonization projects, and other tasks. It's designed to give you quick access to information and streamline certain activities.

# Download
[Latest Release](https://github.com/shalkecsharp/EDA/releases/latest)

# Prerequisites
- Game graphics mode set to BORDERLESS (not mandatory with a second monitor or VR).

# Installation
- Unzip the `.zip` folder anywhere.
- Run `EliteDangerousEase.exe`.
- On the first launch, wait for the journal processing to finish.

# UI Navigation
- Show/Hide with right CTRL.
- Keyboard
    - Right Ctrl shows/hides application.
    - Q,E navigates tabs.
    - W,A,S,D navigates panels.
    - SPACE triggers actions.
    - BACKSPACE navigates back.
- Controller/Joystick
    - Button10 shows/hides application.
    - Button3, Button4 navigates tabs.
    - POV navigates panels.
    - Button1 triggers actions.
    - Button2 navigates back.

# Configuration
- Colonization
    This feature needs a configuration file from Google Drive. Look at the section: How to configure Google Cloud API's. This service is free of charge.
- Plot Route
    This feature needs the following key bindings set in the game:
    - Open galaxy map (O)
    - UI up (W)
    - UI down (S)
    - UI select (SPACE)
    - Galaxy map zoom (Z)
    - If you see (W) or (S) bindings used for the Galaxy Map, remove them or use another keystroke.

# Main Sections

The application is organized into several panels, each serving a specific purpose:

**HOME**: This panel displays informative messages to the user.
- **STATUS**: This panel provides information on current commander status, location, merits, etc.

**FIND**: This panel provides various search types.
- **RECENT LOCATIONS**: This panel provides information on recent visited stations, planets, etc.
- **NEAREST**: This panel provides information on nearest material traders, manufactured materials
- **NEUTRON PLOTTER**: This panel provides information on next jump target based on imported Neutron Plotter webapp plot.
- **INARA**: This panel integrates with the Inara website, providing convenient access to information.

**ENGINEERING**: This panel helps you browse, manage, and pin blueprints.
- **BLUEPRINTS**: This panel provides information and management of engineering process.
- **ENGINEERS**: This panel provides information on engineers.
- **SHIPS**: This panel provides information about your ships including ships and modules info.

**COLONIZATION**: This panel displays and manages colonization projects. (Needs Google Drive configuration)
- **COLONIZATION PROJECTS**: This panel tracks and displays linked colonization projects info.
- **ADD PROJECT**: This panel creates a new colonization project based on docked construction site data.
- **SETTINGS**: This panel configures Google Drive credentials, overlay visibility and manages linked projects.

**MACRO**: This panel displays and manages configuration of different macro patterns that send keystrokes.
- **PATTERN 1**: This panel displays and manages pattern1 script parameters including a keybord shortcut to execute the pattern.

# How to configure Google Cloud API's
