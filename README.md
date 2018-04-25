<div class="post">
<header class="post-header">
<h1 class="post-title">Tunnelbroker.net &amp; ASUS routers</h1>
</header>
<article class="post-content">

<h2 id="the-tunnel">The tunnel</h2>
<p>Go to the router web panel and IPv6 under advanced settings.</p>
<h3 id="basic-config">Basic Config</h3>
<ul>
<li>Connection type: Tunnel 6in4</li>
<li>Server IPv4-address: <em>Server IPv4 Address from IPv6 tunnel endpoints in
tunnelbroker.net tunnel details</em></li>
<li>Client IPv6 address: <em>Client IPv6 address from IPv6 tunnel endpoints in
tunnelbroker.net tunnel details</em></li>
<li>IPv6 prefix length: 64</li>
<li>Tunnel MTU: 0</li>
<li>Tunnel TTL: 255</li>
</ul>
<h3 id="ipv6-lan-setting">IPv6 LAN Setting</h3>
<ul>
<li>LAN IPv6 Prefix: <em>Routed /64 from Routed IPv6 Prefixes from
tunnelbroker.net tunnel details</em></li>
<li>LAN Prefix Length: 64</li>
</ul>
<h3 id="ipv6-dns-setting">IPv6 DNS Setting</h3>
<ul>
<li>IPv6 DNS Server 1: 2001:470:20::2 <em>(this is the one tunnelbroker.net
says for me)</em></li>
<li>IPv6 DNS Server 2: 2001:4860:4860::8888 <em>Google DNS 1</em></li>
<li>IPv6 DNS Server 3: 2001:4860:4860::8844 <em>Google DNS 2</em></li>
</ul>
<h3 id="auto-configuration-setting">Auto Configuration Setting</h3>
<ul>
<li>Enable Router Advertisement: Enable</li>
</ul>
<h2 id="dynamic-dns">Dynamic DNS</h2>
<p>Go to Advanced Settings, WAN, DDNS</p>
<ul>
<li>Enable the DDNS CLient: Yes</li>
<li>Server: WWW.TUNNELBROKER.NET</li>
<li>Host Name: <em>tunnel ID from tunnelbroker.net tunnel details</em></li>
<li>User Name or E-mail address: *username of tunnelbroker.net</li>
<li>Password or DDNS Key: <em>Update Key from tunnel details under the Advanced
tab</em></li>
</ul>
<p>All guides I have seen say that username is user ID from index of
tunnelbroker.net and password is account password, but that doesn’t work
for me. This is how I got it working guessing the details based on
<em>Example Update URL</em> at the same place you got the Update Key.</p>
<p>Now it should either work or not.</p>
<ul>
<li>If it gives error saying something about trying again later, you are
doing something wrong.</li>
<li>If it gives error about endpoint IP not changed since the last update,
it works.</li>
<li>If you don’t get error, it doesn’t work.</li>
</ul>
</article>

</div>
