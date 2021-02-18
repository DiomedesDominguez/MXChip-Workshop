## Installation in Ubuntu

At the time of writting I was using Ubuntu 20.10. When I execute ``` sudo sh -c 'echo "deb [arch=amd64] https://packages.microsoft.com/repos/microsoft-ubuntu-$(lsb_release -cs)-prod $(lsb_release -cs) main" > /etc/apt/sources.list.d/dotnetdev.list' ```

I had to change the ```/etc/apt/sources.list.d/dotnetdev.list``` file to use focal (Ubuntu 20.04) because is the latest version from Microsoft.

### VS Code configuration
Use Ctrl+, to open your settings.json, and add the following lines (use your own username, obviously)

```
    "arduino.path": "/media/diomedes/Data/arduino-1.8.13",
    "arduino.additionalUrls": "https://raw.githubusercontent.com/VSChina/azureiotdevkit_tools/master/package_azureboard_index.json"
```

Use ```Ctrl+Shift+P``` to open the command palette, type and select **Arduino: Board Manager**. Search for **AZ3166** and install the latest version
