# Stream Deck Azure DevOps plugin

Source code of Azure DevOps plugin by Panu Oksala for [Elgato Stream Deck][Stream Deck]. This project works currently only on Windows devices.
Project is created by using the [Stream Deck C# Toolkit][Stream Deck C# Toolkit Homepage].
Use GitHub issues to submit any bugs / feature requests.

## How to use this plugin

Install the plugin from Stream Deck Store and create Azure DevOps PAT token with read & execute permissions to run builds and releases.

### Configurations

**Organization name:** The name of the Azure DevOps organization. The Azure DevOps url contains the organization name and it is best to get it from there: *dev.azure.com/{organization name}.*\
**Project name:** The name of the project like it is in the project URL. Spaces must be replaced with %20. For example "Example Project" is *Example%20Project*\
**PAT:** The personal access token with read and execute permissions for build and release pipelines. Dont create PAT tokens with full access!\
**Pipeline type:** Build or release depending on what kind of action you want to trigger\
**Definition Id:** The build or release definition ID. Open the pipeline in edit mode and copy the ID from URL. For example: *https://dev.azure.com/{organization name}/{projectname}/_apps/hub/ms.vss-ciworkflow.build-ci-hub?_a=edit-build-definition&id={definition ID}*

If the configuration is wrong the Stream Deck button will show exclamation icon indicating that some of the configuration is not correct. Check configuration and try again.\
On success build or release init the Stream Deck button will show OK sign for a short while.
## References

* [Stream Deck C# Toolkit Homepage](https://github.com/FritzAndFriends/StreamDeckToolkit)
* [Stream Deck Page][Stream Deck]
* [Stream Deck SDK Documentation][Stream Deck SDK]

<!-- References -->
[Stream Deck]: https://www.elgato.com/en/gaming/stream-deck "Elgato's Stream Deck landing page for the hardware, software, and SDK"
[Stream Deck C# Toolkit Homepage]: https://github.com/FritzAndFriends/StreamDeckToolkit "C# Stream Deck library"
[Stream Deck software]: https://www.elgato.com/gaming/downloads "Download the Stream Deck software"
[Stream Deck SDK]: https://developer.elgato.com/documentation/stream-deck "Elgato's online SDK documentation"
[Style Guide]: https://developer.elgato.com/documentation/stream-deck/sdk/style-guide/ "The Stream Deck SDK Style Guide"
[Manifest file]: https://developer.elgato.com/documentation/stream-deck/sdk/manifest "Definition of elements in the manifest.json file"


[![.NET](https://github.com/panuoksala/streamdeck-azuredevops-plugin/actions/workflows/dotnet.yml/badge.svg?branch=master)](https://github.com/panuoksala/streamdeck-azuredevops-plugin/actions/workflows/dotnet.yml)
