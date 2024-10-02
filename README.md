# File++
Based on the Home Assistant Core Integrations [`File`](https://www.home-assistant.io/integrations/file/), I created a custom version that reads and writes **multi-line** content. 

**Use case examples:**
- Store and read data larger than 255 characters
- Load email HTML templates
- Store large AI/ChatGPT responses
- ... and much more!

**Features:**
- Use the `notify` service to write multi-line content to a local file. If a file already exists, its content will be erased and the new content will be stored
- Use the `sensor` service to read multi-line content from a local file. The content is available in the `content` attribute of the sensor.

**Removed:**
- State of the `sensor` no longer holds the content of the file. Shows 'Ok' (for now :) ).
- No header is written to empty/new files

# Installation

## 1a. Install via HACS (recommended) 
Publish via HACS in progress..

## 1b. Manual install
1) Download the latest release of the File++ from this repository;
2) In Home Assistant, create a folder `config/custom_components`;
3) Add the File++ files to the `custom_components` folder (you should end up it with a `config/custom_components/file_plusplus` folder);
4) Restart Home Assistant;
5) Add a File++ entity as an Integration in Home Assistant `(menu: settings -> devices & services -> add integration)`;

For updates, repeat step 1 to 4. Home Assistant will not delete any configuration.

# Support
<a href="https://www.buymeacoffee.com/benjamindcs" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" alt="Buy Me A Coffee" style="height: 60px !important;width: 217px !important;" ></a>
