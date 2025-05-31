# Universal-Pet-Microchip-Lookup-Tool

[License: MIT](https://opensource.org/license/MIT)

## Overview
This web application helps identify potential manufacturers or issuing companies of a pet's microchip based on its number format (specifically, its prefix). It serves as a quick reference tool for individuals such as veterinary staff, shelter workers, animal control officers, and concerned citizens who have found a lost pet and are trying to determine the origin of its microchip.

The core data for this tool is meticulously transcribed from the "[MICROCHIP FORMAT GUIDE](https://www.microchiphelp.com/uploads/9/9/7/3/9973230/format_03-29-2025.pdf)" provided by MicrochipHelp.com and Lost Dogs of America. The version of the guide used for this application was last known to be updated on February 4, 2025.

🔴 IMPORTANT DISCLAIMER: This tool DOES NOT check live pet registration databases and CANNOT provide any pet owner information. It only suggests the likely manufacturer or brand associated with the microchip's prefix. Identifying the chip manufacturer is only the first step.

## Table of Contents
- [How to Use](#how-to-use)
- [Live Demo](#live-demo)
- [Features](#features)
- [Data Source](#data-source)
- [Critical Next Steps](#critical-next-steps)
- [Technical Details](#technical-details)
- [Contributing](#contributing)
- [Future Enhancements](#future-enhancements)
- [Acknowledgements](#acknowledgments)
- [License](#license)

## How to Use
 1. Access the Tool:
	 - If hosted online (see Live Demo section), simply navigate to the provided URL.
	 - Alternatively, clone this repository or download the files. Open the index.html file in any modern web browser.
 2. Enter Microchip Number: Type or paste the pet's microchip number (typically 9 to 15 characters, alphanumeric) into the input field. Any spaces, hyphens, or asterisks will be automatically removed during processing.
 3. Lookup: Click the "Lookup Manufacturer" button.
 4. View Results: The application will display:
	 - Potential manufacturer(s) or brand(s).
	 - Available contact information (phone, web, email).
	 - Important notes from the guide (e.g., "info if unenrolled," test chip warnings).
	 - If no specific prefix is matched, guidance on next steps will be provided.

## Live Demo
You can try the live tool here: https://elitegreyit67.github.io/Universal-Pet-Microchip-Lookup-Tool/

## Features
- Prefix-Based Identification: Identifies potential microchip brands/manufacturers using common prefixes.
- Comprehensive Embedded Data: Utilizes a detailed dataset transcribed from the "MICROCHIP FORMAT GUIDE" (MicrochipHelp.com / Lost Dogs of America, updated 02/04/2025).
- Supports Various Formats: Handles 15-digit, 10-digit, and 9-digit microchip numbers, including alphanumeric ones.
- Detailed Information Display: Provides company names, clickable contact details (phone, web, email), and relevant notes.
- Test Chip Warnings: Highlights known test chip patterns.
- User-Friendly Interface: Clean, responsive design built with Tailwind CSS for ease of use on desktop and mobile devices.
- Clear Guidance: Directs users to essential resources like the AAHA Universal Pet Microchip Lookup tool for actual registration searches.
- Client-Side Operation: All processing and data lookup happens directly in the user's browser. No data is sent to or stored on any server.
  
## Data Source
The primary data source for this tool is the "MICROCHIP FORMAT GUIDE" from:
 MicrochipHelp.com (Website: www.microchiphelp.com)
- Lost Dogs of America
The version of the guide used for this application was last known to be updated on February 4, 2025. For questions or information regarding the guide itself, you may try contacting Team@microchiphelp.com.
Limitations:
- The information is static and based on the last known update of the guide. Microchip company details, prefixes, and registry participation can change over time.
- While transcription was done meticulously, errors are possible.
- This tool is not a replacement for official, live database lookups.
Always verify information with official pet recovery services.

## Critical Next Steps
If you have found a lost pet and obtained its microchip number, using this tool to identify the potential chip company is only the very first step. To find the pet's owner, you MUST use comprehensive pet recovery services that search actual registration databases:
1. ✅ AAHA Universal Pet Microchip Lookup: www.petmicrochiplookup.org
   - This is the most crucial resource. It searches multiple major pet recovery service databases in North America.
2. ☑️ PetChip.info: www.petchip.info
   - Some microchip registries do not participate in the AAHA lookup tool. It is highly advisable to also check this database.
 3. 🌍 International Databases (if applicable):
	 - If the chip doesn't seem to be from North America (e.g., doesn't start with '9' or a known US-based AVID format), it might use an ISO Country Code.
	 - Check resources like:
	 - Europetnet: www.europetnet.com
	 - PetMaxx: www.petmaxx.com
	 - List of ISO Country Codes: Wikipedia - ISO 3166-1 numeric
	 - ICAR (International Committee for Animal Recording) for RFID information: www.icar.org

## Technical Details
- Frontend: Vanilla HTML, CSS (Tailwind CSS), and JavaScript.
- Data Storage: Microchip prefix data is stored in microchip_data.json and loaded client-side.
- Dependencies:
	- Tailwind CSS (via CDN) for styling.
	- Font Awesome (via CDN) for icons.
- Operation: Fully client-side; no backend or server interaction is required for the lookup functionality.

## Contributing
While this project primarily serves as a tool based on a static dataset (the "MICROCHIP FORMAT GUIDE"), contributions are welcome:
- Bug Reports: If you find issues with the application's functionality, please open an issue.
- UI/UX Improvements: Suggestions for enhancing the user interface or experience are welcome.
- Data Corrections/Updates: If you have concrete evidence of a discrepancy and can point to an updated, official version of the "MICROCHIP FORMAT GUIDE" from MicrochipHelp.com or Lost Dogs of America, please open an issue with clear details. Updating the `microchip_data.json` file is the primary way to improve data accuracy.
	- *Please do not submit individual chip company updates unless they are reflected in a new version of the master guide*.
- Volunteer with Microchip Hunters: The "MICROCHIP FORMAT GUIDE" also mentions an opportunity to volunteer as a "Microchip Hunter" for those with research skills. If interested, visit: https://form.jotform.com/83140603711950
How to Contribute:
1. Fork the repository.
2. Create a new branch (`git checkout -b feature/YourFeature` or `bugfix/YourBugfix`).
3. Make your changes.
4. Commit your changes (`git commit -m 'Add some feature'`).
5. Push to the branch (`git push origin feature/YourFeature`).
6. Open a Pull Request.
   
## Future Enhancements
- Data from External JSON: (Implemented)
- PWA Features: Add service worker for offline availability (though data would still be static).
- Internationalization (i18n): Translate UI elements if there's demand.
- Theme Toggle: Light/Dark mode.
  
## Acknowledgements
- This tool is made possible by the invaluable work and publicly available "MICROCHIP FORMAT GUIDE" compiled and maintained by MicrochipHelp.com (Contact: Team@microchiphelp.com) and Lost Dogs of America. Their efforts in providing this critical information to help reunite lost pets with their families are deeply appreciated.
- The American Animal Hospital Association (AAHA) for providing the Universal Pet Microchip Lookup tool (petmicrochiplookup.org), an essential resource.
  
## License
This project is licensed under the MIT License. See the LICENSE file for details.
