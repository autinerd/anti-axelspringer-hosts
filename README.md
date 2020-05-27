# Anti Axel Springer hosts file

This file blocks all connections to sites which are from Axel Springer Verlag or have a connection with them.

## How to install

### Windows:

- Paste the content of the file axel-springer-hosts into `%WINDIR%\System32\etc\hosts` (admin rights are neccessary)

### Linux:

- Paste the content of the file axel-springer-hosts into `/etc/hosts` (root rights are neccessary)

### uBlock Origin and other adblock add-ons

- Add `https://raw.githubusercontent.com/autinerd/anti-axelspringer-hosts/master/axelspringer-hosts` to the custom filter lists.

### Android (with root access)

- Install [AdAway](https://github.com/AdAway/AdAway) or similar on your phone, then add the link from [above](#ublock-origin-and-other-adblock-add-ons) to the list of hosts-files.

### Android (without root access)

- Install [Blockada](https://github.com/blokadaorg/blokada) on your phone, then add the link from [above](#ublock-origin-and-other-adblock-add-ons) to the lists in "Ad blocker"

### Pi-hole

- In your [Pi-hole](https://pi-hole.net/) admin interface under Settings > Blocklists add `https://raw.githubusercontent.com/autinerd/anti-axelspringer-hosts/master/axelspringer-hosts` to your blocklists and update Gravity.

## Contributing

When you find a domain which belongs to Axel Springer Verlag and it's not on the list or there is a domain which doesn't belong to Axel Springer Verlag, feel free to open an issue or do a pull request.
