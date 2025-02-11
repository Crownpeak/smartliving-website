<a href="http://www.crownpeak.com" target="_blank">![Crownpeak Logo](./images/logo/crownpeak-logo.png "Crownpeak Logo")</a>

# SmartLiving Website Documentation
The SmartLiving Website ("SmartLiving") is a reference implementation for a static website generation. It serves as a guideline and offers best practices for developers and uses the Tailwind CSS framework.

SmartLiving is provided and an example of code and structure within FirstSpirit.

## Overview
The project has two possible performance settings. In the project setting at CSS Mode, the project is set in Performance or Development:
 - In **Performance** mode, the compiled CSS is used. If there are changes in the template, as well as adjustments of CSS colours, the CSS needs to be compiled again. The guide can be found here: https://tailwindcss.com/docs/installation. The Full Deployment has a script where the generated project is zipped to execute the project with the CLI.
 - In **Development** mode, the Tailwind [Play CDN](https://tailwindcss.com/docs/installation/play-cdn) is added, enabling new templates to be developed directly in FirstSpirit and the design to be displayed on the fly. In this case, over 2 MB of CSS is loaded vs 30 KB in the Performance Mode. It is not recommended to use Development mode for production websites.

Please add your Google Maps API key to the project settings to use the location section. For more information, see: https://developers.google.com/maps/documentation/javascript/get-api-key

An [API key](https://developers.google.com/youtube/v3/getting-started) is required to use the YouTube integration and can be set up in the project component. For more information about the YouTube integration, see: https://github.com/e-Spirit/youtube-dap-integration

## Installation
The project can be imported to your FirstSpirit server using the FSDevTools. FsDevTools can be found here: https://github.com/e-Spirit/FSDevTools/releases

After installation, you can use the following command to import the project to your FirstSpirit server:
```
fs-cli import -c [connection_mode] -port [port] -u "[user_name]" -pwd "[user_password]" -h [hostname] -p "[project_name]" -lm "*:[db_layer_name]" -sd [local_sync_directory]
```
If you want to create a new db layer mapping and don't want to import the project using an existing db layer, please use -lm "*:CREATE_NEW"

### Example:
```
fs-cli import -c HTTP -port 8000 -u "Admin" -pwd "Admin" -h myhost.com -p "SmartLiving Website Reference" -lm "*:FirstSpiritDBA" -sd /home/smartliving-website
```

##  Legal Notices
All Crownpeak documentation is subject to the [MIT license](./LICENSE). FirstSpirit is a trademark of Crownpeak Technology, Inc.

Copyright © 2025 Crownpeak Technology, Inc. All rights reserved.

## Disclaimer
This document is provided for information purposes only. Crownpeak may change the contents hereof without notice. This document is not warranted to be error-free, nor subject to any other warranties or conditions, whether expressed orally or implied in law, including implied warranties and conditions of merchantability or fitness for a particular purpose. Crownpeak specifically disclaims any liability with respect to this document and no contractual obligations are formed either directly or indirectly by this document. The technologies, functionality, services, and processes described herein are subject to change without notice.
 is provided for information purposes only. Crownpeak may change the contents hereof without notice. This document is not warranted to be error-free, nor subject to any other warranties or conditions, whether expressed orally or implied in law, including implied warranties and conditions of merchantability or fitness for a particular purpose. Crownpeak specifically disclaims any liability with respect to this document and no contractual obligations are formed either directly or indirectly by this document. The technologies, functionality, services, and processes described herein are subject to change without notice.