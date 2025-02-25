# C2IntelFeeds
Automatically created C2 Feeds | Also posted via [@drb_ra](https://twitter.com/drb_ra)


* Feeds ( Source/Raw Data courtesy of Censys - https://censys.io/ ) \
 **Search 2.0** has massively improved detection rates on non-standard ports. **Great job Censys Team!**

  By default C2s seen active in the last 7 days are added to the main feed files.

  * `C2 IPs` - Live C2 IP (no frontend or CDN IPs - All bad)
  * `C2 Domains` - All domain names extracted from implants, including domain fronting values and fake Host headers (High abuse of MS, Apple and Google).
  * `C2 Domains Filtered` - Excludes several domains abused in domain fronting, along with fake headers for popular sites. Current filter list see:  `exclusions.rex` file
  * `C2 Domains with URL` - Same as domains and domains filtered but including an extra column with the URI path of the C2
  * `C2 Domains with URL and IP` - Same as domains and domains filtered but including an extra column with the URI path of the C2 and another with the C2 IP 

  Additionally a new 30 day set of feed files was added for any C2 seen live in the last 30 days.
  
* VPN 
  * Nord VPN Exit Nodes

* C2_configs 
  * Detailed CobaltStrike Configuration in CSV and JSON including the following fields:  `FirstSeen,ip,ASN,BeaconType,C2Server,Port,SleepTime,Jitter,Proxy_Behavior,HostHeader,CertificateNames,HttpGet_Metadata,HttpPostUri,HttpPost_Metadata,KillDate,PipeName,UserAgent,Watermark,DNS_Idle,DNS_Sleep` IP reflects the true C2 IP not the one provided in the configuration of the beacon.


<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License</a>.
