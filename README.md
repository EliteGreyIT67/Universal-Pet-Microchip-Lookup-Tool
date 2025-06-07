# Universal-Pet-Microchip-Lookup-Tool

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/license/MIT)
![HTML](https://img.shields.io/badge/language-HTML-blue)

---

## Overview

This web application helps identify potential manufacturers or issuing companies of a pet's microchip based on its number format. It serves as a quick, client-side reference tool for individuals such as veterinary staff, shelter workers, or anyone who finds a lost pet.

The core data for this tool is based on the guide provided by MicrochipHelp.com.

The core data for this tool is transcribed from the “[MICROCHIP FORMAT GUIDE](https://www.microchiphelp.com/uploads/9/9/7/3/9973230/format_03-29-2025.pdf)” by MicrochipHelp.com.

> **IMPORTANT DISCLAIMER:**  
> This tool does **not** check live pet registration databases and **cannot** provide any pet owner information. It only suggests the likely manufacturer or brand associated with a microchip number.  
> **Always use official resources and the "Advanced Help" section for a complete owner lookup.**

---

## Table of Contents

- [How to Use](#how-to-use)
- [Example Usage](#example-usage)
- [Live Demo](#live-demo)
- [Features](#features)
- [Data Source](#data-source)
- [Critical Next Steps](#critical-next-steps)
- [Technical Details](#technical-details)
- [FAQ](#faq)
- [Contributing](#contributing)
- [Future Enhancements](#future-enhancements)
- [Accessibility](#accessibility)
- [Acknowledgements](#acknowledgements)
- [License](#license)

---

## How to Use

1. **Access the Tool:**
    - [Live Demo](#live-demo): Go to the provided URL.
    - Or, clone/download this repository and open `index.html` in any modern web browser.

2. **Enter Microchip Number:**  
   Type/paste the pet's microchip number (usually 9–15 alphanumeric characters). The tool automatically removes spaces, hyphens, or asterisks.

3. **Lookup:**  
   Click the “Lookup Manufacturer” button.

4. **View Results:**  
   The app displays:
   - Potential manufacturer(s) or brand(s)
   - Available contact info (phone, web, email)
   - Important notes (e.g., “info if unenrolled”)
   - A dedicated sidebar with direct links to official lookup registries.
   - An "Advanced Help" section for dead-end or unregistered chips.

---
## Example Usage

| Microchip Number | Example Result                              |
|------------------|--------------------------------------------|
| `985112003627548`| Manufacturer: HomeAgain (Datamars, ISO)    |
| `0A1234567`      | Manufacturer: Avid (US), Contact: [website] |
| `900012345678901`| Manufacturer: Generic ISO, use AAHA lookup  |

*Try these in the demo or your local copy!*

---

## Live Demo

👉 **Try it now:**  
https://elitegreyit67.github.io/Universal-Pet-Microchip-Lookup-Tool/

---

## Features

- **Prefix-Based Identification:** Identifies brands/manufacturers using microchip number prefixes.
- **Comprehensive Data:** Based on the latest guide from MicrochipHelp.com (updated 02/04/2025).
- **Supports Multiple Formats:** 15, 10, and 9-digit microchips; alphanumeric included.
- **Detailed Display:** Clickable contact info, notes, warnings for test chips.
- **User-Friendly:** Clean, responsive two-column layout built with Tailwind CSS.
- **Dark/Light Mode:** Toggle between themes for user comfort.
- **Action-Oriented Guidance:** Directs users to official lookup services and advanced volunteer help.
- **Fully Client-Side:** No data is sent to or stored on any server. Your search is private.

---

## Data Source

The primary data source is the microchip prefix guide curated by:
- MicrochipHelp.com ([website](https://www.microchiphelp.com))
- Lost Dogs of America

_Last updated: February 4, 2025._  
Contact: Team@microchiphelp.com

**Limitations:**
- The embedded information is static and may become outdated.
- Always verify with the official pet recovery services listed in the tool.

---

## Critical Next Steps

If you’ve found a lost pet, use this tool to identify the chip company, then:

1. ✅ **Use the Direct Registry Lookups:**
   The tool provides a list of direct links to major registries (PetLink, HomeAgain, etc.). Use them first

2. ☑️ **AAHA Universal Pet Microchip Lookup:** [www.petmicrochiplookup.org](https://www.petmicrochiplookup.org)  
   Searches many North American pet recovery databases.

3. 🆘 **For Dead-End or Unregistered Chips:**
   Use the resources in the "Advanced Help" section of the tool. This includes forms to request assistance from The Microchip Hunters, a volunteer group that specializes in tracing hard-to-find owners.

4. ☑️ **PetChip.info:**  
   [www.petchip.info](https://www.petchip.info)  
   For registries not in the AAHA tool.

5. 🌎 **International Databases:**  
   - [Europetnet](https://www.europetnet.com)
   - [PetMaxx](https://www.petmaxx.com)
   - [ICAR](https://www.icar.org) (for RFID info)

---

## Technical Details

- **Frontend:** HTML, Tailwind CSS, JavaScript
- **Data:** All microchip prefix data is stored as an embedded JSON object within the index.html file. This makes the tool a single, portable file that works offline.
- **Dependencies:**  
  - Tailwind CSS (CDN)
  - Font Awesome (CDN)
- **Operation:** 100% client-side. All logic runs in the user's browser.

---

## FAQ

**Q: What if my chip isn’t found?**  
A: The tool will guide you to use the universal lookups and advanced help resources. An unknown prefix does not mean the chip is invalid.

**Q: Can I use this offline?**  
A: Because all data is embedded in the index.html file, you can download the repository and open the file locally without an internet connection.

**Q: Is owner info provided?**  
A: No. For privacy and security, this tool only provides likely manufacturer/brand information.

**Q: Is my data private?**  
A: Yes. All lookups are processed locally in your browser; nothing is sent to a server.

---

## Contributing

Contributions are welcome!

- **Bug Reports:** Open an issue if you find a bug.
- **UI/UX Improvements:** Suggest enhancements to the interface or workflow.
- **Data Corrections:** If you have *official* updated info, open an issue or PR.
- **Volunteer:** To help trace chips for found pets, contact The Microchip Hunters via [MicrochipHelp.com](MicrochipHelp.com).

### How to Contribute

1. Fork this repo.
2. Create a branch (`feature/YourFeature` or `bugfix/YourBugfix`).
3. Make your changes and commit.
4. Push your branch and open a pull request.

Please see [CONTRIBUTING.md](CONTRIBUTING.md) if available.

--- 

## Future Enhancements

- [ ] Convert to a PWA (Progressive Web App) for enhanced offline support and "installability."
- [ ] Add internationalization (i18n) to support multiple languages.
- [*] Theme toggle (dark/light mode)
- [ ] Implement an optional external JSON data source that can be updated without editing the HTML.

---

## Accessibility

- The tool is designed for keyboard navigation and screen readers using semantic HTML and ARIA attributes.
- If you encounter any accessibility issues, please open an issue so they can be addressed.
  
---

## Acknowledgements

- “MICROCHIP FORMAT GUIDE” by MicrochipHelp.com & Lost Dogs of America
- American Animal Hospital Association ([AAHA Universal Pet Microchip Lookup](https://www.petmicrochiplookup.org))

---
  
## License

This project is licensed under the MIT License.  
See the [LICENSE](LICENSE) file for details.

