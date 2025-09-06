# Open Source Procurement Guide

A browser-based tool to help government and public sector teams navigate the procurement of Free and Open Source Software (FOSS) solutions. The guide provides step-by-step, jurisdiction-specific best practices, checklists, and sample prompts for each stage of the procurement process.

## Features
- Step-by-step procurement guidance for multiple jurisdictions and languages
- YAML-based, easily editable guidance and prompts for each region
- Save and load progress as YAML files (no data stored on server)
- Dynamic navigation through procurement stages
- LLM prompt suggestions for each stage
- All processing is local in your browser

## Getting Started

### Prerequisites
- Any modern web browser (Chrome, Firefox, Edge, Safari)
- Python 3 (for running a local web server)

### Running Locally
1. Clone or download this repository.
2. In the project directory, start a local web server:
   
   ```sh
   python3 -m http.server
   ```
   
   Or use another static server (e.g. `npx serve`).
3. Open your browser and go to `http://localhost:8000/`.

## Project Structure

- `index.html` — Main application UI and logic
- `jurisdiction/` — YAML files for each region/language (e.g. `us-national.yaml`, `ca-national-en.yaml`)
- `README.md` — This file

## Adding or Editing Guidance
- Edit or add YAML files in the `jurisdiction/` directory.
- Each YAML file contains guidance for all procurement stages and LLM prompts for that region/language.

## Supported Procurement Stages
1. Market Research
2. Planning & Requirements
3. RFP/Tender
4. Evaluation
5. Award & Contracting
6. Implementation
7. Maintenance

## Customization
- To add a new jurisdiction or language, create a new YAML file in `jurisdiction/` and update the mapping logic in `index.html` if needed.
- To change the UI or logic, edit `index.html` directly.

## License
MIT License. See `LICENSE` file for details.

## Credits
- Inspired by open government and digital public infrastructure best practices.
- Uses [js-yaml](https://github.com/nodeca/js-yaml) for YAML parsing in the browser.

---
For questions or contributions, please open an issue or pull request.
