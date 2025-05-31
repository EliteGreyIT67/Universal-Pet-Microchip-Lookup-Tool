# Universal-Pet-Microchip-Lookup-Tool
## Description
This web application helps identify potential manufacturers or issuing companies of a pet's microchip based on its number format (prefix). It is designed as a quick reference tool for individuals trying to determine the origin of a microchip, such as veterinary staff, shelter workers, or concerned citizens who have found a lost pet.
The data used in this tool is meticulously transcribed from the ["MICROCHIP FORMAT GUIDE"](https://www.microchiphelp.com/uploads/9/9/7/3/9973230/format_03-29-2025.pdf) provided by MicrochipHelp.com and Lost Dogs of America (last known update: February 4, 2025).
IMPORTANT: This tool DOES NOT check live pet registration databases and CANNOT provide pet owner information. It only suggests the likely manufacturer or brand based on the chip's prefix.
## How to Use
 * Clone this repository or download the files.
 * Open the index.html file in any modern web browser.
 * Enter the pet's microchip number (9 to 15 characters, alphanumeric) into the input field. Spaces, hyphens, and asterisks will be automatically removed.
 * Click the "Lookup Manufacturer" button.
 * The application will display potential manufacturer(s), contact information, and relevant notes based on the recognized prefix.
## Features
 * Prefix-Based Lookup: Identifies potential microchip brands/manufacturers using common prefixes.
 * Comprehensive Data: Utilizes data from the "MICROCHIP FORMAT GUIDE" (MicrochipHelp.com / Lost Dogs of America, updated 02/04/2025).
 * Multiple Formats: Supports 15-digit, 10-digit, and 9-digit microchip numbers, including alphanumeric ones.
 * Detailed Information: Provides company names, contact details (phone, web, email where available), and important notes (e.g., "info if unenrolled," test chip warnings).
 * User-Friendly Interface: Clean, responsive design for easy use on desktop and mobile devices.
 * Clear Next Steps: Guides users to essential resources like the AAHA Universal Pet Microchip Lookup tool for actual registration searches.
## Data Source
The primary data source for this tool is the "MICROCHIP FORMAT GUIDE" from:
 * MicrochipHelp.com
 * Lost Dogs of America
The version of the guide used for this application was last updated on February 4, 2025.
Critical Next Steps for Finding a Pet's Owner
If you have found a lost pet and obtained its microchip number, this tool is only the first step to identify the potential chip company. To find the pet's owner, you MUST use comprehensive pet recovery services:
 * AAHA Universal Pet Microchip Lookup: www.petmicrochiplookup.org
   * This is the most crucial resource. It searches multiple major pet recovery service databases in North America.
 * PetChip.info: www.petchip.info
   * Some microchip registries do not participate in the AAHA lookup tool. It's advisable to also check this database.
 * International Databases (if applicable):
   * If the chip doesn't seem to be from North America (e.g., doesn't start with '9' or a known US-based AVID format), it might use an ISO Country Code.
   * Check resources like:
     * Europetnet: www.europetnet.com
     * PetMaxx: www.petmaxx.com
     * List of ISO Country Codes: Wikipedia - ISO 3166-1 numeric
## Disclaimer
 * This tool is provided for informational purposes only.
 * The data is based on the "MICROCHIP FORMAT GUIDE" (updated 02/04/2025) and may not be exhaustive or reflect the most current information available from manufacturers or registries. Microchip company information, prefixes, and participation in registries can change.
 * The accuracy of the information provided by this tool is not guaranteed. Always verify with official pet recovery services.
 * This tool does not store any personal data or microchip numbers entered by the user. All processing is done client-side in the browser.
## Contributing
While this project primarily serves as a static data lookup tool based on the aforementioned guide, suggestions for UI improvements or reports of discrepancies (if cross-referenced with an updated version of the official guide) are welcome. Please open an issue in the GitHub repository.
If you have access to a more recent version of the "MICROCHIP FORMAT GUIDE" from MicrochipHelp.com, updating the manufacturersData array in index.html would be the primary way to enhance this tool's accuracy.
## License
This project is licensed under the MIT License. See the LICENSE file for details.

