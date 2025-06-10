# Universal Pet Microchip Lookup Tool

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
![HTML](https://img.shields.io/badge/language-HTML-blue)
[![GitHub issues](https://img.shields.io/github/issues/EliteGreyIT67/Universal-Pet-Microchip-Lookup-Tool)](https://github.com/EliteGreyIT67/Universal-Pet-Microchip-Lookup-Tool/issues)
[![GitHub forks](https://img.shields.io/github/forks/EliteGreyIT67/Universal-Pet-Microchip-Lookup-Tool)](https://github.com/EliteGreyIT67/Universal-Pet-Microchip-Lookup-Tool/network)
[![GitHub stars](https://img.shields.io/github/stars/EliteGreyIT67/Universal-Pet-Microchip-Lookup-Tool)](https://github.com/EliteGreyIT67/Universal-Pet-Microchip-Lookup-Tool/stargazers)

---

## Overview

This web application helps identify the likely manufacturer or brand of a pet's microchip based on its number. It is designed as a quick, client-side reference for veterinary staff, shelter workers, and anyone who has found a lost pet. The core data is transcribed from the “[MICROCHIP FORMAT GUIDE](https://www.microchiphelp.com/uploads/9/9/7/3/9973230/format_03-29-2025.pdf)” by MicrochipHelp.com.

> **IMPORTANT DISCLAIMER:** > This tool does **not** check live pet registration databases and **cannot** provide any pet owner information. It is only a reference to suggest the likely company associated with a microchip number.  
> **Always use official resources like the AAHA Universal Lookup for a complete owner search.**

---

![Application Screenshot](https://imgur.com/79HgsZO.png)
*The Universal Pet Microchip Lookup Tool interface, showing results and next steps.*

---

## 📍 Live Demo

You can use the tool live right now at:
**[https://elitegreyit67.github.io/Universal-Pet-Microchip-Lookup-Tool/](https://elitegreyit67.github.io/Universal-Pet-Microchip-Lookup-Tool/)**

---

## How to Use

1.  **Open the live demo** link above.
2.  **Enter the microchip number** into the input field.
3.  **Click "Lookup Microchip."**
4.  The tool will identify the probable manufacturer and provide notes.
5.  Use the provided links under **"Official Lookups"** and **"Advanced Help"** to continue your search for the pet's owner.

---

## Example Usage

Here are a few examples of what the tool can identify. Try these in the demo!

| Microchip Number | Expected Result from This Tool             |
|------------------|--------------------------------------------|
| `985112003627548`| **Manufacturer:** HomeAgain (Datamars, ISO)    |
| `0A1234567`      | **Manufacturer:** AVID (10-digit)          |
| `900012345678901`| **Note:** Unregistered "900" series ISO chip. Use AAHA lookup. |

---

## 🆘 Critical Next Steps for a Found Pet

If you have found a lost pet, use this tool to identify the chip company, then follow these steps:

1.  ✅ **Use the AAHA Universal Pet Microchip Lookup:**
    * [**www.petmicrochiplookup.org**](https://www.petmicrochiplookup.org) — This should be your first stop. It searches most major North American pet recovery databases at once.

2.  ☑️ **Try the Direct Registry Lookups:**
    * If AAHA doesn't yield a result, use the direct links provided by this tool (e.g., PetLink, HomeAgain) based on the identified manufacturer.

3.  🆘 **For Dead-End or Unregistered Chips (Advanced Help):**
    * Use the resources in the **"Advanced Help"** section of the tool. This includes a link to request assistance from **The Microchip Hunters**, a volunteer group that specializes in tracing hard-to-find owners.

4.  🌐 **Check Other Databases:**
    * **International:** [Europetnet](https://www.europetnet.com), [PetMaxx](https://www.petmaxx.com)
    * **Other Lookups:** [PetChip.info](https://www.petchip.info) (for registries not in the AAHA tool)

---

## ✨ Features

- **Prefix-Based Identification:** Identifies brands/manufacturers using the microchip number.
- **Comprehensive Data:** Based on the latest guide from MicrochipHelp.com (updated 02/04/2025).
- **Supports Multiple Formats:** Handles 15, 10, and 9-digit microchips, including alphanumeric ones.
- **Detailed Display:** Shows manufacturer, clickable contact info, and important notes.
- **User-Friendly:** Clean, responsive layout built with Tailwind CSS.
- **Dark/Light Mode:** Toggle between themes for user comfort.
- **Action-Oriented:** Guides users directly to official lookup services and expert volunteer help.
- **Fully Client-Side:** Your search is private. No data is sent to or stored on any server.

---

## 🛠️ Technical Details & Local Setup

- **Frontend:** HTML, Tailwind CSS (via CDN), Font Awesome (via CDN), and vanilla JavaScript.
- **Data:** All microchip prefix data is stored as an embedded JSON object within `index.html`. This makes the tool a single, portable file that works offline.
- **Operation:** 100% client-side. All logic runs in the user's browser.

To run this project on your local machine:

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/EliteGreyIT67/Universal-Pet-Microchip-Lookup-Tool.git
    ```
2.  **Navigate to the project directory:**
    ```bash
    cd Universal-Pet-Microchip-Lookup-Tool
    ```
3.  **Open the `index.html` file** in your web browser.

---

## ❓ FAQ

**Q: Can I use this offline?** A: Yes. Because all data is embedded in the `index.html` file, you can download the repository and open the file locally without an internet connection.

**Q: Does this tool show owner information?** A: **No.** For privacy and security, this tool only provides likely manufacturer/brand information to guide your next search steps.

**Q: What if the chip number isn't found in this tool?** A: An unknown prefix does not mean the chip is invalid. It simply means it's not in our reference guide. You should **always** proceed to the "Critical Next Steps" and use the AAHA universal lookup.

---

## 🤝 Contributing

Contributions are welcome!

- **Bug Reports & Data Corrections:** If you find a bug or have *official* updated information on a chip prefix, please [open an issue](https://github.com/EliteGreyIT67/Universal-Pet-Microchip-Lookup-Tool/issues).
- **UI/UX Improvements:** Suggest enhancements to the interface or workflow.
- **Volunteer to Find Pets:** To help trace chips for found pets, contact The Microchip Hunters via [MicrochipHelp.com](https://www.microchiphelp.com/).

### How to Contribute Code

1.  Fork this repository.
2.  Create a new branch (`git checkout -b feature/YourAmazingFeature`).
3.  Make your changes and commit them (`git commit -m 'Add some AmazingFeature'`).
4.  Push to the branch (`git push origin feature/YourAmazingFeature`).
5.  Open a Pull Request.

---

## 🚀 Future Enhancements

- [ ] Convert to a Progressive Web App (PWA) for enhanced offline support.
- [ ] Add internationalization (i18n) to support multiple languages.
- [x] Theme toggle (dark/light mode).
- [ ] Implement an optional external JSON data source for easier updates.

---

## Acknowledgements

- **“MICROCHIP FORMAT GUIDE”** by MicrochipHelp.com & Lost Dogs of America
- **American Animal Hospital Association** ([AAHA Universal Pet Microchip Lookup](https://www.petmicrochiplookup.org))

---

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

