# Media Server Package

There are many applications that lets you easily manage your home media library. This section focuses on getting some of those applications installed properly in your system.

1. You will first be asked where to store the applications' data. This will then be updated as the storage location for all the config files.

Example is provided below, you can either go for the same or change as per your needs.

```sh
/data/docker
```

Few things to note:
 -  You should not include the trailing '/' when you type in to the script.
 -  Each application will be created as a sub directory within the specified folder.

So if you have provided "/data/docker" to be the path, the Plex application will be installed under "/data/docker/plex".

2. Then you'd need to provide the desired paths for the Movies, TV Shows and Downloads.

You need to provide the path for the directories in which the media files are stored. If you do not have any media files, just provide the path to the drive in which you have a lot of free space. You can use `df -h` command to take a look at your system's free space and partitions.

3. That's it. From now on, it is just a matter of pressing either 'y' or 'n' to the applications to install.


The list of apps that can be installed are:

- Plex – For organizing and streaming the media content (https://www.plex.tv/)
- Tautulli – A simple tool to monitor plex activity and collect the statistics (https://tautulli.com/)
- Sonarr – A collection manager for web series (https://sonarr.tv/)
- Radarr – A collection manager for movies (https://radarr.video/)
- Sabnzbd – A USENET client/downloader (https://sabnzbd.org/)
- Deluge – A torrent tracker and downloader (https://deluge-torrent.org/)
- Overseerr – A media discovery and request manager for Plex (https://overseerr.dev)
- Jackett – A bridge for apps listed above to communicate with the torrent indexers of your choice (https://github.com/Jackett/Jackett)
- Watchtower – A container to automatically update all the application containers listed above (https://github.com/containrrr/watchtower)

Once you finish making your choices, the script will start by initializing the system updates, followed by Docker, Docker Compose, Portainer and the list of apps chosen.

You will be seeing what operations are being carried out and are also provided with the URL to start setting up and using the application.

When the installation completes, I suggest that you visit the Portainer's URL (https://yourip:9443) and set up the admin account. 

Once logged in, you need to set up your admin account, and you'll be presented with the dashboard.

![portainer](https://user-images.githubusercontent.com/101336634/158015527-e7d01b42-03b8-4f4f-b0a3-0d343b685a37.png)

The system has successfully processed the installation if you see this page. You can now play with your new setup and start configuring the applications as per your liking.
