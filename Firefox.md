# My typical firefox setup  

# Profiles:  

Accessed and created in about:profiles   
Commandline for choosing which profile to launch, ProfileName is case sensitive (Works on both Windows and GNU/linux):  
`firefox -P ProfileName`

## Daily usage profile  

### about:config tweaks    
(If a boolean does not exist, use the + button to create one and choose the right option)

**Prevent WebRTC leak:**  
media.peerconnection.enabled = false

**Prevent browser fingerprinting**  (can break things)  
privacy.resistfingerprinting = true

**Disable TLS false start**  
security.ssl.enable_false_start = false

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

I use **medium mode**. Will cause (very slight) breakage but after a few days of using it all my sites that I use regularly were working with no problems. After that it's a matter of copying custom rules/filters over.

## Decentraleyes
"It prevents a lot of requests from reaching networks like Google Hosted Libraries, and serves local files to keep sites from breaking. Complements regular content blockers."
The description pretty much sums it up.

## Bitwarden
Free and open source password manager. The android app is better than Last Pass's and it offers some great features. Integrates into the browser as well as the context menu. 



