# Country DNS filter catalog

AdAway is the sole global default. Each country below has one selected canonical DNS/hosts source, discovered through adblocklists.com and cross-checked against upstream documentation/AdGuard's hostlist registry where appropriate. This is a supported-country catalog, not coverage of every nation or an assertion that every blocked domain belongs to that country.

The native compiler normalizes/deduplicates domains and encodes sorted 64-bit SHA-256 prefixes. Browser cosmetic/path/conditional/IP rules are excluded. Sources containing unsupported allow exceptions are rejected, including unsafe historical fallbacks. Current artifacts reproduce byte-for-byte from their retained source snapshots.

| Country code | Selected source | Domains at this build | License | Canonical source |
| --- | --- | ---: | --- | --- |
| VN | Vietnam · hostsVN | 18,537 | [MIT](https://raw.githubusercontent.com/bigdargon/hostsVN/master/LICENSE) | [DNS source](https://raw.githubusercontent.com/bigdargon/hostsVN/master/hosts) |
| CN | China · anti-AD | 108,290 | [MIT](https://raw.githubusercontent.com/privacy-protection-tools/anti-AD/master/LICENSE) | [DNS source](https://raw.githubusercontent.com/privacy-protection-tools/anti-AD/master/anti-ad-domains.txt) |
| JP | Japan · hosts-jp Ads | 1,729 | [CC-BY-4.0](https://raw.githubusercontent.com/tiuxo/hosts/master/LICENSE) | [DNS source](https://raw.githubusercontent.com/tiuxo/hosts/master/ads) |
| KR | South Korea · YousList | 625 | [CC-BY-4.0](https://github.com/yous/YousList#license) | [DNS source](https://raw.githubusercontent.com/yous/YousList/master/hosts.txt) |
| PL | Poland · Polish Pi-hole | 1,140 | [CC-BY-NC-SA-4.0](https://raw.githubusercontent.com/MajkiIT/polish-ads-filter/master/LICENSE) | [DNS source](https://raw.githubusercontent.com/MajkiIT/polish-ads-filter/master/polish-pihole-filters/hostfile.txt) |
| SE | Sweden · Frellwit | 1,155 | [GPL-3.0](https://raw.githubusercontent.com/lassekongo83/Frellwits-filter-lists/master/LICENSE) | [DNS source](https://raw.githubusercontent.com/lassekongo83/Frellwits-filter-lists/master/Frellwits-Swedish-Hosts-File.txt) |
| TR | Turkey · Turkish Ad Hosts | 2,071 | [GPL-3.0](https://raw.githubusercontent.com/symbuzzer/Turkish-Ad-Hosts/main/LICENSE) | [DNS source](https://raw.githubusercontent.com/symbuzzer/Turkish-Ad-Hosts/main/adguard/filter.txt) |
| ID | Indonesia · ABPindo | 125 | [GPL-3.0-or-later](https://raw.githubusercontent.com/ABPindo/indonesianadblockrules/master/LICENSE) | [DNS source](https://raw.githubusercontent.com/ABPindo/indonesianadblockrules/master/subscriptions/aghome.txt) |
| IR | Iran · PersianBlocker | 258 | [AGPL-3.0](https://raw.githubusercontent.com/PersianBlocker/PersianBlocker/main/LICENSE) | [DNS source](https://raw.githubusercontent.com/PersianBlocker/PersianBlocker/main/PersianBlockerHosts.txt) |
| NO | Norway · Nordic Hosts | 479 | [Dandelicence-1.4](https://raw.githubusercontent.com/DandelionSprout/adfilt/master/LICENSE.md) | [DNS source](https://raw.githubusercontent.com/DandelionSprout/adfilt/master/NorwegianExperimentalList%20alternate%20versions/NordicHosts.txt) |
| HU | Hungary · Hufilter DNS | 92 | [CC-BY-4.0](https://raw.githubusercontent.com/hufilter/hufilter/master/LICENSE) | [DNS source](https://raw.githubusercontent.com/hufilter/hufilter/gh-pages/hufilter-dns.txt) |
| LT | Lithuania · EasyList Hosts | 54 | [GPL-3.0](https://raw.githubusercontent.com/EasyList-Lithuania/easylist_lithuania/master/LICENSE) | [DNS source](https://raw.githubusercontent.com/EasyList-Lithuania/easylist_lithuania/master/EasyListLithuaniaHosts.txt) |
| BD | Bangladesh · Malicious Hosts BD | 25 | [BSD-3-Clause](https://raw.githubusercontent.com/touhidurrr/malicious-hosts-bd/main/LICENSE) | [DNS source](https://raw.githubusercontent.com/touhidurrr/malicious-hosts-bd/main/domains.txt) |
| MK | North Macedonia · Macedonian Pi-hole | 210 | [Upstream-redistribution-permission](https://raw.githubusercontent.com/cchevy/macedonian-pi-hole-blocklist/master/hosts.txt) | [DNS source](https://raw.githubusercontent.com/cchevy/macedonian-pi-hole-blocklist/master/hosts.txt) |
| TH | Thailand · ThaiConsentHosts | 9,098 | [CC-BY-NC-4.0](https://raw.githubusercontent.com/kowith337/ThaiConsentHosts/master/license.md) | [DNS source](https://raw.githubusercontent.com/kowith337/ThaiConsentHosts/master/ThaiConsentHosts.txt) |

AdAway: 6,540 domains; CC BY 3.0, with original contributor attribution. Total: 16 artifacts including 15 country choices. All sixteen binary files together are about 1.21 MB; a device still permits at most five installed lists including paused/default lists.

Selection limits: Norway's Nordic source also covers Denmark/Iceland/Faroese sites upstream, but is offered only once under NO to avoid duplicate installations. Bangladesh's source focuses on malicious domains rather than comprehensive advertising. Lithuania's upstream DNS variant describes itself as small/alpha. PL is CC BY-NC-SA 4.0 and TH is CC BY-NC 4.0; these data files retain those noncommercial terms. Full notices and original snapshots are distributed alongside artifacts. Country lists are optional supplements; they can contain overlapping global domains.

No country-code/TLD blanket blocklists, stale third-party browser conversions or fabricated empty lists were selected. Countries without an appropriate verified DNS source remain unsupported. AdGuard DNS and HaGeZi Light are removed from new discovery, while their old immutable files and already-installed owner copies remain intact and manageable.

On existing ESPs install the new firmware and choose **Làm mới danh sách**. Catalog refresh changes discovery only; it does not enable, delete or install sources automatically. Use the country name (Vietnamese or English), source name or ISO code to search. Updates of installed retired lists are no longer offered; toggle/removal remain local. Do not reflash data partitions.
