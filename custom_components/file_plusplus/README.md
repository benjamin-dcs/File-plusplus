## 1a. Install via HACS (recommended)
Will add to HACS if there's any interest. Create an [issue](https://github.com/benjamin-dcs/home-assistant/issues) to indicate interest.

## 1b. Manual install
1) Download the latest release of the File++ from this repository;
2) In Home Assistant, create a folder `config/custom_components`;
3) Add the File++ files to the `custom_components` folder (you should end up it with a `config/custom_components/file_plusplus` folder);
4) Restart Home Assistant;
5) Add a File++ entity as an Integration in Home Assistant `(menu: settings -> devices & services -> add integration)`;

For updates, repeat step 1 to 4. Home Assistant will not delete any configuration.
