# Liberty Server: More private file sharing, made simple(ish)

## Why use Liberty Server?
With a growing trend of authoritarianism around the globe, keeping your web traffic concealed is more of a concern than ever.
This is including, and especially concerning, the dissemination of information many regimes may not like, such as:
- Political organizing handbooks
- International legal codes
- Great works of public domain, subversive literature
- Software useful to free oneself of intrusive monitoring and censorship
Using torrent software, aware activists can rapidly distribute such critical information with little necessary infrastructure.

### Why develop Liberty Server?
See above, but getting some basic practice in Docker was useful.

## Dependencies
- [Qbittorrent](https://hub.docker.com/r/linuxserver/qbittorrent), a BitTorrent protocol server
- [Gluetun](https://hub.docker.com/r/qmcgaw/gluetun), a Dockerized VPN client container designed to make it easier to connect other containers to VPNs

## TODO
- Solve bug where Gluetun can't update filter block lists from AirVPN
- Figure out if qBittorrent passwords can be set at start
- Gluetun already has a healthcheck function, but it would be nice to write a script to verify that we're in the allowed IP range