# Devcontainer-Ruby

This is my take on a ruby devcontainer. The Microsoft one includes a couple
deprecated extensions that can't be removed easily. In addition, I wanted some
other options for ruby versions and build tools.

### Current Ruby Version: 3.2.2

devcontainer.json
```
{
    "name": "Ruby",
    // Or use a Dockerfile or Docker Compose file. More info: https://containers.dev/guide/dockerfile
    "image": ""

    // Features to add to the dev container. More info: https://containers.dev/features.
    // "features": {},

    // Use 'forwardPorts' to make a list of ports inside the container available locally.
    // "forwardPorts": [],

    // Use 'postCreateCommand' to run commands after the container is created.
    // "postCreateCommand": "ruby --version",

    // Configure tool-specific properties.
    // "customizations": {},

    // Uncomment to connect as root instead. More info: https://aka.ms/dev-containers-non-root.
    // "remoteUser": "root"
}
```
