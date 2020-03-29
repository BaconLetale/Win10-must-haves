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


