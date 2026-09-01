---
layout: default
title: "Horizon Summary: 2026-09-01 (EN)"
date: 2026-09-01
lang: en
---

> From 11 items, 5 important content pieces were selected

---

1. [Google removes Manifest V2 extensions, including uBlock Origin, from Chrome Web Store.](#item-1) ⭐️ 8.0/10
2. [DIY project repurposes security camera audio feeds into an automated bird identification system using BirdNET-Go.](#item-2) ⭐️ 7.0/10
3. [Personal account raises concerns about potential hack of military commissary freezers](#item-3) ⭐️ 7.0/10
4. [Article argues NAT was a foundational cause of internet centralization.](#item-4) ⭐️ 7.0/10
5. [Introducing Wrapture: A Python library for unified tracing and mocking.](#item-5) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Google removes Manifest V2 extensions, including uBlock Origin, from Chrome Web Store.](https://webiterate.dev/google-removed-extensions-ublock-origin-108/) ⭐️ 8.0/10

Google has removed all Manifest V2 extensions from the Chrome Web Store, including the widely-used ad blocker uBlock Origin. This action forces users and developers to transition to the newer, more restrictive Manifest V3 standard. This move significantly impacts the ad-blocking ecosystem and user privacy, as Manifest V3 limits the capabilities of content-blocking extensions. It consolidates Google&\#x27;s control over the browser extension landscape, potentially affecting millions of users who rely on powerful ad blockers for safety and a cleaner web experience. The removal is part of a phased deprecation timeline; while users can currently re-enable disabled MV2 extensions, a future phase will permanently prevent this. Notably, uBlock Origin&\#x27;s developer has stated the extension works best on Firefox, which supports the more capable MV2 standard.

hackernews · twapi · Aug 31, 21:10 · [Discussion](https://news.ycombinator.com/item?id=49514878)

**Background**: Browser extensions require a manifest.json file that defines their capabilities and permissions. Manifest V2, introduced in 2012, has been the standard for over a decade, allowing extensions like uBlock Origin to use the powerful \`webRequest\` API for dynamic content filtering. Manifest V3, introduced by Google, replaces this with a more restrictive \`declarativeNetRequest\` API, limiting how extensions can inspect and modify web traffic, which is crucial for advanced ad blockers.

<details><summary>References</summary>
<ul>
<li><a href="https://developer.chrome.com/docs/extensions/develop/migrate/mv2-deprecation-timeline">Manifest V2 support timeline | Chrome for Developers</a></li>
<li><a href="https://dev.to/notearthian/whats-the-difference-between-manifest-v2-and-v3-in-browser-extensions-3b10">What&#x27;s the Difference Between Manifest V2 and V3 in browser extensions? - DEV Community</a></li>
<li><a href="https://factually.co/fact-checks/technology/manifest-v3-ad-blockers-ublock-origin-brave-firefox-2026-4d29ee">How Manifest V 3 Changed Ad Blockers: uBlock Origin, Br...</a></li>

</ul>
</details>

**Discussion**: The community expresses strong concern and frustration, viewing the move as a safety issue and an overreach of corporate control. Many commenters advocate switching to Firefox, citing its continued support for Manifest V2 and better compatibility with uBlock Origin. There is a shared sentiment of nostalgia for Chrome&\#x27;s early days and a resolve to resist what is seen as Google&\#x27;s unilateral control over web standards.

**Tags**: `#browser-extensions`, `#ad-blocking`, `#chrome`, `#web-standards`, `#privacy`

---

<a id="item-2"></a>
## [DIY project repurposes security camera audio feeds into an automated bird identification system using BirdNET-Go.](https://jasontucker.blog/how-i-turned-my-security-cameras-into-an-automatic-bird-identification-system-with-birdnet-go/) ⭐️ 7.0/10

A blog post detailed a method to transform standard security camera audio feeds into a continuous bird monitoring system by using the self-hosted BirdNET-Go software for real-time, local AI inference. The project leverages existing RTSP streams from cameras like Ubiquiti&\#x27;s Unifi doorbell to &\#x27;listen&\#x27; and classify bird sounds. This demonstrates a creative, low-cost application of AI that makes advanced bioacoustic monitoring accessible to hobbyists and homeowners, turning common IoT devices into scientific tools. It highlights the growing trend of repurposing consumer hardware for environmental sensing and citizen science projects. The BirdNET-Go software performs local AI inference and is designed for 24/7 real-time soundscape analysis. A key technical challenge mentioned is that BirdNET expects 48kHz audio samples, and some camera microphones may only support lower sampling rates \(e.g., 16kHz\), which can affect identification accuracy or require workarounds like using an external microphone.

hackernews · speckx · Aug 31, 16:47 · [Discussion](https://news.ycombinator.com/item?id=49511856)

**Background**: BirdNET is a state-of-the-art AI system developed by Cornell University that uses a convolutional neural network to identify wildlife vocalizations from short audio segments. Many modern IP security cameras support the Real-Time Streaming Protocol \(RTSP\), which allows their video and audio feeds to be accessed by third-party software. BirdNET-Go is a self-hosted, open-source implementation of this technology that enables continuous, local analysis without sending data to the cloud.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/tphakala/birdnet-go">GitHub - tphakala/ birdnet - go : Self-hosted realtime soundscape...</a></li>
<li><a href="https://birdnet.cornell.edu/">BirdNET – AI-Powered Sound ID</a></li>
<li><a href="https://bou.org.uk/blog-granados-birdnet/">How to use BirdNET - British Ornithologists&#x27; Union</a></li>

</ul>
</details>

**Discussion**: The community discussion shows strong interest and practical engagement, with users sharing their own implementations using different camera brands \(Unifi, Aqara\) and highlighting technical hurdles like audio sampling rates and wind noise. Several commenters extended the concept by building portable units with e-ink displays for field use and sharing links to their own setup guides and 3D-printable cases.

**Tags**: `#DIY`, `#Machine Learning`, `#IoT`, `#BirdNET`, `#Home Automation`

---

<a id="item-3"></a>
## [Personal account raises concerns about potential hack of military commissary freezers](https://signalandsilence.substack.com/p/i-think-someone-hacked-the-commissary) ⭐️ 7.0/10

A personal account published online suggests that industrial freezers in a U.S. military commissary may have been compromised, leading to widespread malfunctions. The incident sparked a detailed discussion on Industrial Control System \(ICS\) security and supply chain vulnerabilities. This incident highlights the potential vulnerability of critical infrastructure, even in military settings, to cyber attacks targeting operational technology. A successful attack on such systems could disrupt essential supply chains, impact local economies, and pose significant safety risks. The author acknowledges that the malfunctions could also be due to misconfiguration or maintenance issues, not necessarily a deliberate hack. Community experts note that isolated overseas locations like Guam or Hawaii could be higher-value targets for such attacks due to their greater logistical impact.

hackernews · jcurbo · Aug 31, 11:45 · [Discussion](https://news.ycombinator.com/item?id=49508506)

**Background**: Industrial Control Systems \(ICS\), which include SCADA and DCS, are used to monitor and control industrial processes in critical infrastructure like power grids and water treatment plants. Programmable Logic Controllers \(PLCs\) are common components within ICS that are often criticized for having outdated software, weak default security \(like admin/admin credentials\), and a lack of encryption, making them vulnerable to cyber attacks. Supply chain attacks target these systems by compromising trusted vendors or software updates to infiltrate secure environments.

<details><summary>References</summary>
<ul>
<li><a href="https://www.tripwire.com/solutions/industrial-control-systems">ICS Security | Industrial Cybersecurity Control Systems</a></li>
<li><a href="https://plcprogramming.io/blog/plc-security-best-practices-complete-guide">PLC Security Best Practices Guide</a></li>
<li><a href="https://panorays.com/blog/cyber-security-supply-chain-attacks/">Cyber Security Supply Chain Attacks: Navigating the 2026 Threat Landscape</a></li>

</ul>
</details>

**Discussion**: Community sentiment is mixed, with some experts considering a misconfiguration more likely than a hack, while others find the scenario plausible based on firsthand experience with insecure PLCs. Comments provide historical context on supply chain vulnerabilities and share anecdotes about the poor security practices commonly found in industrial control systems, such as contractors not enabling TLS and using default passwords.

**Tags**: `#Cybersecurity`, `#Industrial Control Systems`, `#Critical Infrastructure`, `#Supply Chain`, `#PLC Security`

---

<a id="item-4"></a>
## [Article argues NAT was a foundational cause of internet centralization.](https://dreamstation.systems/personal/ntppost.html) ⭐️ 7.0/10

An article posits that Network Address Translation \(NAT\) was a foundational cause of internet centralization by eroding the ability for users to easily host servers and normalizing the client-server model. The article&\#x27;s critique has sparked debate, including a comment from Rusty Russell, the implementer of Linux&\#x27;s NAT system, who acknowledged its role in removing public endpoints. This perspective challenges a core networking technology often taken for granted, linking a technical design decision to profound societal outcomes like the dominance of cloud platforms and the decline of peer-to-peer, user-hosted services. It reframes the debate about internet architecture, highlighting the trade-offs between security, address conservation, and the original end-to-end principle of openness. The article specifically criticizes how NAT&\#x27;s design, which prioritizes multiplexing outgoing connections over a single IP, inherently blocks unsolicited incoming traffic, making servers behind NAT unreachable without explicit port forwarding. A key counterpoint in the discussion is that Carrier-Grade NAT \(CGNAT\) is seen as more restrictive than standard NAT, and that poor user experience \(UX\) for port forwarding, not NAT itself, is a major barrier.

hackernews · robinpie · Aug 31, 02:23 · [Discussion](https://news.ycombinator.com/item?id=49504905)

**Background**: Network Address Translation \(NAT\) is a technique that allows multiple devices on a private network to share a single public IP address for internet access, primarily to conserve the limited pool of IPv4 addresses. The original internet architecture was built on the &\#x27;end-to-end principle,&\#x27; which envisioned that intelligence and control \(like hosting servers\) resided at the network&\#x27;s endpoints \(user devices\), not in the middle. This facilitated a more decentralized, peer-to-peer model, contrasting with the now-dominant client-server model where users \(clients\) primarily consume services from centralized providers \(servers\).

<details><summary>References</summary>
<ul>
<li><a href="https://www.geeksforgeeks.org/computer-networks/network-address-translation-nat/">Network Address Translation ( NAT ) - GeeksforGeeks</a></li>
<li><a href="https://devopedia.org/end-to-end-principle">End - to - End Principle</a></li>
<li><a href="https://en.wikipedia.org/wiki/Peer-to-peer">Peer - to - peer - Wikipedia</a></li>

</ul>
</details>

**Discussion**: The community discussion reveals nuanced views on NAT&\#x27;s impact. Rusty Russell, who implemented Linux&\#x27;s NAT, expressed regret that his design eliminated public endpoints. Others, like elric, argue that calling NAT the &\#x27;original sin&\#x27; is an exaggeration, distinguishing regular NAT from the more restrictive Carrier-Grade NAT \(CGNAT\) and blaming poor UX for port forwarding. A sentiment emerged that NAT provided a crucial, if imperfect, security layer for vulnerable devices, highlighting the complex trade-off between accessibility and protection.

**Tags**: `#networking`, `#internet-history`, `#decentralization`, `#nat`, `#architecture`

---

<a id="item-5"></a>
## [Introducing Wrapture: A Python library for unified tracing and mocking.](https://simonwillison.net/2026/Aug/31/introducing-wrapture/) ⭐️ 7.0/10

Graham Dumpleton has released Wrapture, a new Python library that extends the monkeypatching concepts from his \`wrapt\` library to enable simultaneous, non-invasive tracing and mocking of functions and methods. The project, just a few weeks old, includes OpenTelemetry support and a configuration-based mechanism for adding tracing to existing projects. This matters because it addresses a persistent challenge in Python development: observing and testing code, especially third-party or legacy code, without modifying its source. By unifying tracing \(for observability\) and mocking \(for testing\), Wrapture offers a powerful tool for developers working on debugging, performance monitoring, and creating robust test suites. Wrapture provides an alternative to Python&\#x27;s standard \`unittest.mock\` and can be configured via TOML files to attach tracing to specific targets. Notably, the entire project, including its code and documentation, was written by an AI assistant under Graham Dumpleton&\#x27;s careful direction and engineering, distinguishing it from less controlled &\#x27;vibe coding&\#x27; approaches.

rss · Simon Willison · Aug 31, 23:59

**Background**: Monkey patching is a technique in Python that allows developers to modify or extend the behavior of functions, methods, or classes at runtime without altering the original source code. Graham Dumpleton&\#x27;s \`wrapt\` library is a well-known tool for performing reliable monkey patching. Separately, \`unittest.mock\` is a standard library module for replacing parts of a system under test with mock objects, and OpenTelemetry is a vendor-neutral framework for collecting telemetry data like traces and metrics.

<details><summary>References</summary>
<ul>
<li><a href="https://wrapt.readthedocs.io/en/develop/monkey.html">Monkey Patching — wrapt 2.4.0 documentation</a></li>
<li><a href="https://github.com/GrahamDumpleton/wrapt">GitHub - GrahamDumpleton/wrapt: A Python module for decorators ...</a></li>
<li><a href="https://realpython.com/python-mock-library/">Understanding the Python Mock Object Library – Real Python</a></li>

</ul>
</details>

**Tags**: `#python`, `#testing`, `#observability`, `#libraries`

---