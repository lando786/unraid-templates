# Trilium Notes docker template for Unraid

This repository contains the xml file with docker the template to add Trilium Next Notes Server as a Community Application to Unraid.

## About the template

This template allows the installation of the Trilium Next Notes Server as a docker container from Unraid's Community Application.
It contains the latest stable version.

This templates configures the host port as `9999` since the default container port `8080` is wildly used.
There are also two configuration paths: the `/home/node/trilium-data` directory with the default `/mnt/user/appdata/trilium` and the optional path for `/home/node/trilium-data/backup`. In case the path for the backups isn't provided they will be present in `/mnt/user/appdata/trilium/backup`. This definition is useful in case you want to setup a backup utility from the unraid pool and not the cache (where the `appdata` is stored).

## Notes

If you have or had Trilium previously installed this should use the same directories and your instance should contain all your notes. If you decide to change the paths manually and want to keep your old notes, look into Trilium Next documentation section for [Importing/Exporting Markdown](https://github.com/TriliumNext/Docs/blob/main/Wiki/markdown.md)


## About Trilium

Trilium Notes is a hierarchical note taking application with focus on building large personal knowledge bases.

### Builds

- [Latest release](https://github.com/TriliumNext/Notes/releases/latest) 
- [Docker image](https://hub.docker.com/r/triliumnext/notes)

### Documentation

[Trilium Next Documentation.](https://github.com/TriliumNext/Docs/)
