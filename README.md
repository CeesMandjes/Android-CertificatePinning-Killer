# Android-CertificatePinning-Killer

Frida code modification script which can be used to bypass certificate pinning in an Android environment [1]. Using this script, all the certificates will be considered as trusted. The following certificate pinning libraries can be bypassed with this script:
<ul>
<li>Android's default library</li>
<li>OKHttp library</li>
</ul>

Frida works on both nonrooted and rooted Android device. This script is tested on the TLSConnector [2,3].

Usage: frida -U -l bypassCertificatePinningAndroid.js -f org.package.name --no-pause

[1] = https://frida.re/ <br/>
[2] = https://gitlab.local.northwave.nl/cmandjes/tlsconnector <br/>
[3] = https://gitlab.local.northwave.nl/cmandjes/tlsconnectorserver <br/>