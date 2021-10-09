# home-router

Ansible config for my home router, an AVM FRITZ!Box 4040.

My home router expects primary internet connectivity on the wired WAN Ethernet port. Generally I'll have the router plugged into whatever shitty ISP box is available. My iPhone is automatically tethered when it's plugged into the USB port, and its internet is used if the primary WAN is unavailable (courtesy of mwan3).

Regardless of how I'm connected to the internet, all Internet traffic egresses from my router via a Mullvad Wireguard tunnel. Mullvad's DNS resolver is also used to prevent DNS leaks.

Tailscale is also configured and running, so I can always securely connect to my router (and my home network) from anywhere.
