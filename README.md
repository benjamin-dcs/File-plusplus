# File++
Based on the Home Assistant Core Integrations [`File`](https://www.home-assistant.io/integrations/file/), I created a custom version that reads and writes **multi-line** content. I personally use this to load email-templates and store data larger than 255 characters (which is the max of a Text Helper (any entity for that matter)).

**Features:**
- Use the `notify` service to write multi-line content to a local file
- Use the `sensor` service to read multi-line content from a local file. The content is available in the `content` attribute of the sensor.

**Removed:**
- State of the `sensor` no longer holds the content of the file. Shows 'Ok' (for now :) ).
- No header is written to empty/new files

# Support
<a href="https://www.buymeacoffee.com/benjamindcs" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" alt="Buy Me A Coffee" style="height: 60px !important;width: 217px !important;" ></a>
