# Google Summer of Code 2025 

### Chromium: Debug WebUI for Tabstrip States

| Role | Description |
|------|--------------|
| **Organization** | The Chromium Project |
| **Mentors** | [Darryl James](https://chromium-review.googlesource.com/q/owner:dljames@chromium.org), [Shibalik Mohapatra](https://chromium-review.googlesource.com/q/owner:shibalik@chromium.org), [Atharv Maan](https://chromium-review.googlesource.com/q/owner:atharvmaan@chromium.org) |
| **Contributor** | [Brijesh Giri](https://chromium-review.googlesource.com/q/owner:brijeshvgiri@gmail.com) |
| **Project Area** | Desktop Top Chrome |
| **Duration** | May – August 2025 |

## Project Summary

This project implements a **read-only WebUI page** in Chromium (chrome://tab-strip-internals) that provides a live, structured visualization of the **tabstrip model**, including tab groups, selection state, and session-restore metadata.

The WebUI helps developers debug and inspect complex tab behaviors by exposing internal C++ model data from the TabStripModel, TabRestore Service, and Session Service through a **Mojo interface** and rendering it in a **TypeScript-based frontend**.

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

## Key Links

| Resource | Description |
|-----------|-------------|
| [Project Proposal](https://docs.google.com/document/d/e/2PACX-1vRxbZNAwQaeUCgdnjFE9greSpvEhY9ikNFrr4Bx2XUt5TZ6xYlrZY64dA2ijjXdW6Vd2DadDBgmB68s/pub) <br> | The original GSoC proposal that was selected. <br> (Future contributors can refer to this.) |
| [Presentation Slides](https://docs.google.com/presentation/d/1flYoOy7ZYUmdnPUZ1WZG4AbTBqxyrEihbS9rJepRhp4/edit?usp=sharing) <br> | Mid-project presentation summarizing progress and findings. |
| [Buganizer Issue](https://issues.chromium.org/issues/427204855) <br> | Google's internal issue tracker entry for project tracking during GSoC. |
| [Contributor Gerrit](https://chromium-review.googlesource.com/q/owner:brijeshvgiri@gmail.com) <br> | All related Chromium code reviews (Gerrit). |

## How to Access

To access the developed feature, launch Chromium with the feature flag:

    out/Default/chrome --enable-features=DebugUITabStrip

Open the page:

    chrome://tab-strip-internals

## TODO: Add Demo GIF

TODO: Add recorded demo, screenshots, or GIFs  <br/>
Example:

- Demo GIF: (Add embedded gif here) 
- Screenshot Gallery: demo/

## Repository Contents

| File / Folder | Description |
|---------------|-------------|
| README.md | Project summary and documentation |
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
