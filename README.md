# LLuviaOS
## Official builds application

Before pushing the update, you should know a few simple things:

### 1. Hosting

Our files are hosted on [SourceForge](https://sourceforge.net/projects/lluviaos-3-0/)

### 2. Changelog
For each new version, you need to upload the changelog to this repository in the device specific folder.

The changelog file name must match the **.zip** file name and should end with **.txt**
Eg: **.zip** is **LLuviaOS-v3.0-Crystal-ham-NatureMade-20190210.zip**, changelog file name should be **LLuviaOS-v3.0-Crystal-ham-NatureMade-20190210.txt**

### 3. Addons
You can add links to device specific addons(firmwares patches, tweaks, hotfixes etc) in [addons.json](https://github.com/LLuviaDevices/official_builds/blob/3.0/addons.json) , it will appear inside OTA app. Make sure to follow the syntax and
avoid adding duplicate addons that already exists in **default** array, those are universal addons that can be used on all the devices.

### 4. Over-the-air (OTA) updates
Our system is automatic, you should not worry about updating some script, just upload the new build to the [SourceForge](https://sourceforge.net/projects/lluviaos-3-0/) and edit your device JSON file (**builds/your_device_codename.json**) in this repository and also upload the changelog txt.

Eg: Moto G 2015 is called **osprey**, so the device JSON file is **builds/osprey.json**

**Note:** New builds can take up to 30 minutes to appear on the site and in the OTA application.

### 5. JSON parameters
| Param | Description | Required |
|--|--|--|
| addons | Device specific addons | No |
| developer | Your Name | Yes |
| developer_url | Your personal URL(Git or xda) | No |
| forum_url | XDA thread URL | Yes |
| filename | Latest build name | Yes |
| build_date | Date Of your Build, eg 20190210 | Yes |
| filesize | Size of your build | Yes |
| md5 | md5 Code of your zip | Yes |
| url | Link to download, eg https://sourceforge.net/projects/lluviaos-3-0/files/ham/LLuviaOS-v3.0-Crystal-ham-NatureMade-20190210.zip/download | Yes |
| version | LLuviaOS version | Yes |

Example: [Click here](https://github.com/LLuviaDevices/official_builds/blob/3.0/builds/ham.json)

**Please format your JSON code properly, [here](https://jsonformatter.curiousconcept.com/).**

### 6. Build type
You need to add 'export LLUVIA_BUILD_TYPE=OFFICIAL' in your build environment so that the OTA app will be included in your build.

### 7. Device tree
Maintainers should upload their device trees on https://github.com/LLuviaDevices

### Important Links:

- [Website](https://www.lluvia.ga/)
- [Download Center](https://downloads.aospextended.com/)
- [Apply for Official Device](https://goo.gl/forms/lad1qDHLKttcffei2)
- [Telegram Channel](https://telegram.me/LLuvia_Os/)
- [Official Devices](https://github.com/LLuviadevices/)
