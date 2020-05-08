# Basic Code Flow for 802.11 connection in Linux
* Mode: _Station_
* Security: _None_

Steps of connection completion:
1. Probe Request (Active Scanning) / (Passive Scanning)
2. Probe Response / Beacon (Scan Results)
3. Authentication Request
4. Authentication Response
5. Association Request
6. Association Response

Layers:
* [wpa_supplicant](https://w1.fi/wpa_supplicant/)
* cfg80211 - [`/net/wireless`](https://github.com/torvalds/linux/tree/master/net/wireless)
* mac80211 - [`/net/mac80211`](https://github.com/torvalds/linux/tree/master/net/mac80211)
* driver - [`/drivers/net/wireless/ath/ath9k`](https://github.com/torvalds/linux/tree/master/drivers/net/wireless/ath/ath9k)

# Source Code Used (Version Details)
* Linux Version: `5.4.31`
* wpa_supplicant: `2.10`
