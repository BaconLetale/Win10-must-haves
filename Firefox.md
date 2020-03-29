# My typical firefox setup  

# Profiles:  

## Daily usage profile  

### about:config tweaks  

**Prevent WebRTC leak:**  
media.peerconnection.enabled

**Prevent browser fingerprinting**  
privacy.resistfingerprinting = true

**Disable TLS false start**  
security.ssl.enable_false_start = false

**3DES has known security flaws, so it's good to disable it**  
security.ssl3.rsa_des_ede3_sha = false

**Require safe negotiation**  
security.ssl.require_safe_negotiation = true

**Prevent usage of old TLS**  
security.tls.version.min = 3  
security.tls.version.max = 4

**Disable 0 round trip time**  
security.tls.enable_0rtt_data = false 

**Disable Automatic Formfill, rarely used, insecure and annoying**  
browser.formfill.enable = false

**Disable geolocation**  
geo.enabled = false

**Disable plugin scanning. Can by itself prevent adblocker detection among other things**.  
plugin.scan.plid.all = false

**Disable telemetery**  
browser.newtabpage.activity-stream.feeds.telemetry = false
browser.newtabpage.activity-stream.telemetry = false
browser.pingcentre.telemetry = false
devtools.onboarding.telemetry-logged = false
media.wmf.deblacklisting-for-telemetry-in-gpu-process = false
toolkit.telemetry.archive.enabled = false
toolkit.telemetry.bhrping.enabled = false
toolkit.telemetry.firstshutdownping.enabled = false
toolkit.telemetry.hybridcontent.enabled = false
toolkit.telemetry.newprofileping.enabled = false
toolkit.telemetry.unified = false
toolkit.telemetry.updateping.enabled = false
toolkit.telemetry.shutdownpingsender.enabled = false


## Privacy oriented profile(can and WILL cause some sites to break)

I just use this user.js file and then tweak the user settings to my liking
https://github.com/pyllyukko/user.js/
The user.js file goes to the profile directory (easily accessible via about:profiles page)

# Extensions

## Ublock Origin
This is always my first install. Blocks ads, many trackers, can be used to zap any part of the page, has custom rules, many filter lists to subscribe too. An absolute must have for any browser.

I use **easy mode(default)** for daily browsing + some language specific filter lists.
I use **medium mode** for the privacy oriented profile. Will cause breakage but an intermiediate user should have no trouble unbreaking any site.

## Privacy Badger
Good companion to Ublock Origin. It's not AS useful with the config tweaks, especially on the privacy profile, but it's good for daily usage. It differs from other extensions in that it learns by observing scripts and figuring out which one follows you and which one does not. Has some defaults of course. The learning nature of this extension means breakage occurs less than with other similar extensions. It's easy to disable it too in case something breaks.

## HTTPS Everywhere
A no brainer extensions. It ensures that all communications are encrypted with the HTTPS protocol. Can be enforced. No reason to not install this extensions. It's even included in the Tor Browser bundle by default.

## Decentraleyes
"It prevents a lot of requests from reaching networks like Google Hosted Libraries, and serves local files to keep sites from breaking. Complements regular content blockers."
The description pretty much sums it up.

## Bitwarden
Free and open source password manager. The android app is better than Last Pass's and it offers some great features. Integrates into the browser as well as the context menu. 

## ScriptSafe(advanced tool, do not use in daily setup)



