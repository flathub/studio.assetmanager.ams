# Installing from the flathub.org repository
See https://flathub.org/apps/details/studio.assetmanager.ams for details.

# Local build
- Use `flatpak run org.flatpak.Builder --force-clean --sandbox --install-deps-from=flathub --ccache --repo=repo --user --mirror-screenshots-url=https://dl.flathub.org/media/ --install builddir studio.assetmanager.ams.yaml` command to build & install the app into the local `repo` repository. 
- Use `flatpak run studio.assetmanager.ams` command to start the app.
- Use `flatpak remove --delete-data studio.assetmanager.ams` to remove the app.

# Notes 
- The metadata file is located in BuildResources/studio.assetmanager.ams.metainfo.yaml 
  - login to flathub to see if any issues are present and fix them before building the .deb and uploading it to the ams site.
  
- To update the flathub version:
  - update the "studio.assetmanager.ams.metainfo.yaml" file
  - create a new branch and create a pull request.
  - verify the pull request output
  - merge the pull request
