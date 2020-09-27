English version [below](#anti-axel-springer-hosts-file)

# Anti-Axel-Springer-Hostsdatei

Diese Datei blockiert alle Verbindungen zu Webseiten, die entweder dem Axel Springer Verlag gehören oder eine Verbindung mit diesem haben

## Installation

### Windows (ohne weitere Tools, benötigt Adminrechte)

- Inhalt der Datei `axel-springer-hosts` in die Datei `%WINDIR%\System32\etc\hosts` einfügen

### Linux/macOS (ohne weitere Tools, benötigt root-Rechte)

- Inhalt der Datei `axel-springer-hosts` in die Datei `/etc/hosts` einfügen

### uBlock Origin und andere Werbeblocker-Addons

- Füge `https://raw.githubusercontent.com/autinerd/anti-axelspringer-hosts/master/axelspringer-hosts` zu den benutzerdefinierten Filterlisten hinzu

### Android (mit Rootrechten)

- Installiere [AdAway](https://github.com/AdAway/AdAway) oder ähnliches auf das Gerät, danach füge den Link von [oben](#ublock-origin-und-andere-werbeblocker-addons) in die Liste der Hostsdateien hinzu.

### Android (ohne Rootrechte)

- Installiere [Blockada](https://github.com/blokadaorg/blokada) auf das Gerät, im Menü unter "Werbeblocker" füge den Link von [oben](#ublock-origin-und-andere-werbeblocker-addons) in die Liste der Hostslisten hinzu

### Pi-Hole

- Auf der Adminoberfläche unter "Group management" > "Adlists" für den Link von [oben](#ublock-origin-und-andere-werbeblocker-addons) zu den Listen hinzu.

### iOS ([AdGuard](https://apps.apple.com/de/app/adguard-adblock-privacy/id1047223162))

Nicht vergessen den Content Blocker für Safari zu aktivieren

#### Ohne Subscription
  - Öffne die AdGuard settings -> Safari Protection -> User rules
  - Lade die [ios-adguard.txt](https://raw.githubusercontent.com/autinerd/anti-axelspringer-hosts/master/ios-adguard.txt) runter
  - importiere diese Datei in die User Rules

#### Mit Subscription
  - Füge `https://raw.githubusercontent.com/autinerd/anti-axelspringer-hosts/master/axelspringer-hosts` zu den benutzerdefinierten Filterlisten hinzu


## Unterstützen

Wenn Sie eine Domain finden, die nicht auf der Liste ist, aber zu Axel Springer gehört oder aber eine Domain, die nicht zu Axel Springer gehört aber auf der Liste ist, öffnen Sie einfach ein Issue oder ein Pull Request.

Beachten Sie, dass Domains, die auch mit "www." verfügbar sind (wie b\*\*d.de -> www.b\*\*d.de), in die Datei `www-hostnames` gehören, andere in die `hostnames`.

Bei Pull Requests: Nach dem Hinzufügen von Domains bitte `python ./generate_hostfile.py` ausführen.

Natürlich hilft auch ein Teilen dieser Liste an Bekannte und Freunde!

# Anti Axel Springer hosts file

This file blocks all connections to sites which are from Axel Springer Verlag or have a connection with them.

## How to install

### Windows (without further tools, needs admin permissions):

- Paste the content of the file axel-springer-hosts into `%WINDIR%\System32\etc\hosts`

### Linux/macOS (without further tools, needs admin permissions):

- Paste the content of the file axel-springer-hosts into `/etc/hosts`

### uBlock Origin and other adblock add-ons

- Add `https://raw.githubusercontent.com/autinerd/anti-axelspringer-hosts/master/axelspringer-hosts` to the custom filter lists.

### Android (with root access)

- Install [AdAway](https://github.com/AdAway/AdAway) or similar on your phone, then add the link from [above](#ublock-origin-and-other-adblock-add-ons) to the list of hosts-files.

### Android (without root access)

- Install [Blockada](https://github.com/blokadaorg/blokada) on your phone, then add the link from [above](#ublock-origin-and-other-adblock-add-ons) to the lists in "Ad blocker"

### Pi-hole

- In your [Pi-hole](https://pi-hole.net/) admin interface under "Group management" > "Adlists" add `https://raw.githubusercontent.com/autinerd/anti-axelspringer-hosts/master/axelspringer-hosts` to your blocklists and update Gravity.

### iOS ([AdGuard](https://apps.apple.com/de/app/adguard-adblock-privacy/id1047223162))

Don't forget to activate the Content Blocker for Safari

#### without subscription
  - open the AdGuard settings -> Safari Protection -> User rules
  - download [ios-adguard.txt](https://raw.githubusercontent.com/autinerd/anti-axelspringer-hosts/master/ios-adguard.txt)
  - import this file to the User Rules

#### with Subscription
  - Add `https://raw.githubusercontent.com/autinerd/anti-axelspringer-hosts/master/axelspringer-hosts` to the custom filter lists.


## Contributing

When you find a domain which belongs to Axel Springer Verlag and it's not on the list or there is a domain on the list which doesn't belong to Axel Springer Verlag, feel free to open an issue or do a pull request.

Please be aware, that domains which have a "www." counterpart (like b\*\*d.de -> www.b\*\*d.de) has to be in the `www-hostnames`, other domains in the `hostnames` file.

For pull requests: After adding the domains, please run `python ./generate_hostfile.py`

Of course sharing the list helps a lot as well!
