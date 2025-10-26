# Google Summer of Code 2025 

### Chromium: Debug WebUI for Tabstrip States

**Organization:** The Chromium Project  
**Mentors:** [Darryl James](https://chromium-review.googlesource.com/q/owner:dljames@chromium.org), [Shibalik Mohapatra](https://chromium-review.googlesource.com/q/owner:shibalik@chromium.org), [Atharv Maan](https://chromium-review.googlesource.com/q/owner:atharvmaan@chromium.org)  
**Contributor:**
[Brijesh Giri](https://chromium-review.googlesource.com/q/owner:brijeshvgiri@gmail.com)  
**Project Area:** Desktop Top Chrome

**Project Duration:** May – August 2025

## Project Summary

This project implements a **read-only WebUI page** in Chromium (chrome://tab-debug) that provides a live, structured visualization of the **tabstrip model**, including tab groups, selection state, and session-restore metadata.

The WebUI helps developers debug and inspect complex tab behaviors by exposing internal C++ model data through a **Mojo interface** and rendering it in a **Lit-based TypeScript frontend**.

### Key Features
- Real-time updates of the tabstrip model  
- Collapsible tree view showing tabs, groups, and session data  
- Raw data toggle for deep inspection  
- Strictly **read-only** access to maintain browser safety

## Goals

- Create a WebUI chrome page similar to chrome://tab-search.top-chrome/  
- Visualize the tabstrip model as a hierarchical tree  
- Display group and selection model metadata  
- Integrate session information from session restore  
- Ensure complete read-only access (no modification actions)

## Non-Goals

- Performing any state-changing actions from the WebUI  
- Fixing existing tabstrip/session bugs (debug-only focus)

## How To Access

To launch Chromium with the feature flag:

    out/Default/chrome --enable-features=DebugUITabStrip

Open the page:

    chrome://tab-strip-internals

## Key Links

- Proposal: https://docs.google.com/document/d/e/2PACX-1vRxbZNAwQaeUCgdnjFE9greSpvEhY9ikNFrr4Bx2XUt5TZ6xYlrZY64dA2ijjXdW6Vd2DadDBgmB68s/pub  
- Presentation: https://docs.google.com/presentation/d/1flYoOy7ZYUmdnPUZ1WZG4AbTBqxyrEihbS9rJepRhp4/edit?usp=sharing
- Issue Tracker - Buganizer (Google's internal issue tracker): https://issues.chromium.org/issues/427204855

## TODO: Add Demo GIF

TODO: Add recorded demo, screenshots, or GIFs  
Example:

- Demo GIF: (Add embedded gif here) 
- Screenshot Gallery: demo/

## Repository Contents

| File / Folder | Description |
|---------------|-------------|
| README.md | Project summary and documentation |
| docs/ | Proposal, presentation, and static assets |
| patches/ | Gerrit CLs submitted during GSoC |
| demo/ | Screenshots or GIF demos of the WebUI |

## Acknowledgments

Special thanks to my mentors for their constant support and technical guidance throughout the project:

- **[Darryl James](https://chromium-review.googlesource.com/q/owner:darryljames%2540chromium.org)**
- **[Shibalik Mohapatra](https://chromium-review.googlesource.com/q/owner:shibalik%2540chromium.org)**
- **[Atharv Maan](https://chromium-review.googlesource.com/q/owner:atharvmaan%2540chromium.org)**

Thanks also to the Chromium community for maintaining an incredible open-source ecosystem and for their reviews and discussions throughout the GSoC period.

## License

This repository and accompanying documentation are shared publicly for archival and educational purposes.  
All Chromium-related code remains under the **BSD license** as governed by the Chromium project.
