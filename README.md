
# Hi, I'm Christoph Komenda

**UX/UI Designer · Frontend Developer · E-Commerce & Open Source Contributor**

I design and build intuitive digital experiences where **user-centered design, frontend engineering and measurable outcomes** meet — from e-commerce journeys to locally integrated hardware.

My work spans **conversion-focused e-commerce experiences** and **hardware-validated open-source integrations** — turning complex requirements into clear, practical solutions.

[**Portfolio**](https://christophkomenda.de) · [**Resume / CV**](https://christophkomenda.de/wp-content/uploads/2026/10/CV_Christoph_Komenda.pdf) · [**Open-source projects**](https://github.com/ChristophKomenda?tab=repositories)

**Explore selected work:** [Pironman 5](#pironman-5--5-max--home-assistant-integration) · [Weishaupt WTC](#weishaupt-wtc--protocol-reverse-engineering--upstream-contributions) · [E-Commerce](#dnatestch--uxui--e-commerce-relaunch) · [SunFounder IR](#sunfounder--upstream-contributions) · [Bitcoin Pi Node](#bitcoin-pi-node--secure-self-hosted-bitcoin-core)

---

## Selected work

### Pironman 5 / 5 Max — Home Assistant Integration

**Open Source · Python · Home Assistant · HACS · REST API · Docker · Raspberry Pi**

Designed, developed, and maintain an open-source Home Assistant integration that enables **native monitoring and hardware control for SunFounder Pironman 5 / 5 Max** devices.

Built with **Home Assistant Container (Docker)** in mind, the integration bridges the gap between SunFounder's local hardware API and Home Assistant's native entities — without additional cloud services, MQTT, or a separate Home Assistant add-on.

**🏆 Key milestone: Official HACS acceptance**

Successfully reviewed, approved, and merged into the **HACS default repository**, allowing users to discover, install, and update the integration directly through HACS.

**Recent milestone: v1.5.0 — experimental native IR / HAIR receiver support**

The integration now includes an optional native Home Assistant infrared receiver for the **Pironman 5 Max**, connected via a separately installed Linux/LIRC host bridge. It was tested with HAIR on real hardware; the IR capability remains experimental, receive-only and disabled by default. Version 1.4.0 also introduced expanded network and device diagnostics with capability-aware model detection, without claiming verified Pro Max support.

**Key engineering contributions**

- **Native hardware integration:** CPU, GPU, memory, dynamically discovered NVMe / USB storage, network monitoring, and cooling status.
- **Advanced device controls:** Fan profiles, RGB lighting effects, brightness, colors, and OLED display settings.
- **Container-first architecture:** Works with Home Assistant Container and supports network-based communication across separate devices.
- **Configurable REST API:** Adjustable host, port, and polling interval with fully local communication.
- **Open-source quality:** GitHub Actions validation, versioned releases, contribution guidelines, security documentation, and structured issue templates.
- **Hardware compatibility:** Published a model-specific test matrix and capability-aware detection, distinguishing maintainer-tested Pironman 5 Max hardware from unverified models.
- **Optional infrared reception:** Home Assistant `InfraredReceiverEntity`, HAIR integration and a documented host-side LIRC bridge for Pironman 5 Max.

**Verified environment:** Pironman 5 Max with Home Assistant Container. Pironman 5 is a target model; additional Pironman variants require hardware validation.

**Impact:** Expanded Home Assistant integration options for Pironman users, especially those running Docker-based installations, and established a maintainable foundation for future hardware support and community contributions.

[**Explore project & installation →**](https://github.com/ChristophKomenda/pironman5-homeassistant-container) · [IR / HAIR documentation](https://github.com/ChristophKomenda/pironman5-homeassistant-container/blob/main/docs/native-ir-hair.md) · [HACS acceptance](https://github.com/hacs/default/pull/12242) · [Hardware compatibility & testing](https://github.com/ChristophKomenda/pironman5-homeassistant-container/blob/main/docs/hardware-testing.md) · [Latest release](https://github.com/ChristophKomenda/pironman5-homeassistant-container/releases/latest)

### Weishaupt WTC — Protocol Reverse Engineering & Upstream Contributions

**Open Source · Python · Reverse Engineering · CanApiJson · Home Assistant · Hardware Validation · Automated Testing**

Researching and extending the local **Weishaupt WEM / CanApiJson protocol** to make heating-system data more accessible, transparent and useful for monitoring and energy-efficiency analysis.

Using a real **Weishaupt WTC-GW 15-B**, I investigated and hardware-validated 12 heating-circuit (HK1) settings and explored additional boiler-related sensor registers.

**🏆 Key milestone: Three upstream pull requests merged — 24 read-only sensors**

Three contributions have been reviewed and merged into the upstream [kraiz/hassio-weishaupt](https://github.com/kraiz/hassio-weishaupt) repository, most recently on November 21, 2026:

- [**PR #21 — HK1 Heating Curve Monitoring**](https://github.com/kraiz/hassio-weishaupt/pull/21) — Added read-only sensors for heating curve slope and parallel shift.
- [**PR #22 — 10 Additional HK1 Settings**](https://github.com/kraiz/hassio-weishaupt/pull/22) — Added hardware-validated heating circuit configuration sensors, protocol improvements, regression tests and documentation.
- [**PR #24 — 12 WTC Boiler & Pump Sensors**](https://github.com/kraiz/hassio-weishaupt/pull/24) — Added read-only burner, blower and pump diagnostics with automated tests, documented limitations and backward-compatible integration.

**Result:** 24 additional read-only sensors merged upstream (12 HK1 + 12 WTC), expanding heating-system visibility while preserving existing entities and avoiding controller write operations.

**🔬 Key engineering contributions**

- **Heating-circuit monitoring:** Validated heating curve slope, parallel shift, minimum and maximum flow-temperature targets, summer/winter switching thresholds, frost protection and additional HK1 configuration parameters.
- **Protocol reverse engineering:** Identified undocumented CanApiJson register mappings and request/response behavior through direct hardware measurements.
- **Protocol compatibility:** Implemented independent request and response value sizes for selected registers while preserving existing sensor behavior.
- **Regression testing:** Added automated tests covering register addresses, scaling, signed decoding, response validation and backward compatibility.
- **Hardware validation:** Used repeated read-only probes, physical controller comparisons and controlled A-B-A measurements.
- **Boiler sensor expansion:** Added 12 WTC sensors upstream in [PR #24](https://github.com/kraiz/hassio-weishaupt/pull/24), covering burner modulation, blower operation, pump performance and diagnostic parameters.
- **Additional protocol research:** Proposed 13 WTC sensor candidates with regular 60-second polling in [JS-DE-Tech PR #14](https://github.com/JS-DE-Tech/hacs-weishaupt-lan/pull/14).
- **Safety-first implementation:** Preserved entity identifiers, avoided unverified controller write operations and documented known hardware compatibility limitations.

**Selected hardware observations**

| Parameter | Register | Validated observation |
| --- | --- | --- |
| Heating curve slope | `0x254B` | Controller-matched values using × 0.1 scaling |
| Heating curve parallel shift | `0x25AD` | Controller-matched values using × 0.1 scaling |
| Minimum / maximum flow target | `0x251B` / `0x251C` | 15.0 °C / 80.0 °C |
| Summer/winter switching | `0x257B` | 16.0 °C |
| Internal pump electrical power | `0x261B` | 11 W matched controller display |
| Heating pump output limits | `0x256B` / `0x256C` | 30% / 80% |
| Burner target output | `0x2542` | Controller-matched percentage |
| Blower control signal | `0x257E` | Controller-matched percentage |

**Upstream contribution snapshot — November 23, 2026**

| Project | Status | Contributions |
| --- | --- | --- |
| [kraiz/hassio-weishaupt](https://github.com/kraiz/hassio-weishaupt) | **3 merged** | [#21](https://github.com/kraiz/hassio-weishaupt/pull/21), [#22](https://github.com/kraiz/hassio-weishaupt/pull/22), [#24](https://github.com/kraiz/hassio-weishaupt/pull/24) |
| [JS-DE-Tech/hacs-weishaupt-lan](https://github.com/JS-DE-Tech/hacs-weishaupt-lan) | **6 open** | [#9–#14](https://github.com/JS-DE-Tech/hacs-weishaupt-lan/pulls?q=is%3Apr+author%3AChristophKomenda) |
| [BorgNumberOne/Weishaupt_CanApiJson](https://github.com/BorgNumberOne/Weishaupt_CanApiJson) | **2 open** | [#9](https://github.com/BorgNumberOne/Weishaupt_CanApiJson/pull/9), [#10](https://github.com/BorgNumberOne/Weishaupt_CanApiJson/pull/10) |

**Validation scope:** Research findings are based on one WTC-GW 15-B installation. Additional device models, firmware versions and provisional register interpretations require further validation. Long-term polling stability and live integration testing of the newly merged WTC sensors remain outstanding.

**Impact:** Transforming undocumented heating-controller behavior into tested, documented and upstream-accepted open-source functionality that other Home Assistant users and developers can build upon.

[**Merged upstream contributions →**](https://github.com/kraiz/hassio-weishaupt/pulls?q=is%3Apr+author%3AChristophKomenda) · [WTC sensor expansion](https://github.com/JS-DE-Tech/hacs-weishaupt-lan/pull/14) · [Hardware research](https://github.com/ChristophKomenda/hacs-weishaupt-lan/blob/feat/wtc-13-candidates-sammelpr/docs/wtc-gw15b-canapijson-observations-2026-11-10.md)

### DNATest.ch — UX/UI & E-Commerce Relaunch

**UX/UI · WordPress · WooCommerce · HTML · CSS · JavaScript · SEO · CRO**

Redesigned and optimized a Swiss DNA-testing e-commerce experience, focusing on clarity, trust, accessibility of product information and the path from discovery to purchase.

- Reworked content hierarchy, navigation, product presentation and calls to action
- Improved responsive layouts and reusable frontend components
- Implemented structured data and technical SEO enhancements
- Focused on page performance, usability and conversion-oriented journeys

[**Explore DNATest.ch →**](https://dnatest.ch)

### SR Brennholzhandel — Local Business Website Optimization

**Web Design · WordPress · Frontend · Local SEO · GA4 · CRO**

Built and optimized a regional firewood supplier's digital presence to make products, delivery details and contact options easier to understand and act on.

- Improved information architecture and mobile user journeys
- Introduced prominent contact options and conversion-focused calls to action
- Implemented structured data and analytics event tracking
- Worked on frontend performance and technical SEO

[**Visit SR Brennholzhandel →**](https://sr-brennholz.de)

### SunFounder — Upstream Contributions

**Open Source · Raspberry Pi · Linux · Hardware Integration · Home Assistant · IR / LIRC**

Contributing hardware-focused improvements to SunFounder's ecosystem, connecting Linux-level functionality with reproducible smart-home integrations.

**Selected upstream and community contributions**

- [**Pironman 5 Max IR Receiver — upstream PR #26 (closed, not merged)**](https://github.com/sunfounder/home-assistant-addon/pull/26) — Proposed a standalone HAOS infrared receiver add-on and companion integration; independently tested with Home Assistant OS and HAIR.
- [**Official community add-on listing — PR #27 (open)**](https://github.com/sunfounder/home-assistant-addon/pull/27) — SunFounder proposed linking to the community-maintained IR add-on from its official README rather than taking on maintenance of another official add-on.
- [**OLED / SSD1306 Font Asset Fix**](https://github.com/sunfounder/pm_auto/pull/19) — Corrected an asset path issue in the upstream driver.
- [**Debian Trixie Compatibility**](https://github.com/sunfounder/pironman5/pull/109) — Contributed tested platform compatibility information.

**Key technical milestone:** Demonstrated an end-to-end local IR receiving pipeline using the Pironman 5 Max's built-in receiver, GPIO13, LIRC and HAIR. The functionality has also been integrated into my own [Pironman 5 Home Assistant integration](https://github.com/ChristophKomenda/pironman5-homeassistant-container), with an optional host bridge.

**Maintainer feedback:** SunFounder appreciated the documentation, automated tests and independent HAOS validation. They declined merging the standalone add-on due to maintenance scope and manual companion-integration installation, while offering an official **community-maintained project reference** through PR #27. That proposed listing is not yet merged.

**Impact:** Translating device-specific hardware capabilities into locally usable and documented integrations, while making maintenance ownership and deployment limitations transparent.

[**Explore SunFounder IR proposal →**](https://github.com/sunfounder/home-assistant-addon/pull/26) · [Community listing PR](https://github.com/sunfounder/home-assistant-addon/pull/27) · [Native IR / HAIR integration](https://github.com/ChristophKomenda/pironman5-homeassistant-container/blob/main/docs/native-ir-hair.md)

### Bitcoin Pi Node — Secure Self-Hosted Bitcoin Core

**Open Source · Raspberry Pi 5 · Linux · Docker Compose · Bash · systemd · GitHub Actions**

Built a lightweight deployment for a **pruned, validating Bitcoin Core node** on Raspberry Pi 5, with dedicated microSD, SSD or NVMe storage, safer startup controls and optional Home Assistant monitoring.

**Key engineering contributions**

- **Safer startup:** Optional systemd service verifies the mounted filesystem UUID before starting the container, reducing the risk of writing blockchain data to the system drive.
- **Lean architecture:** Configurable pruning, persistent storage and Bitcoin P2P networking without exposing the RPC port on the host.
- **Home Assistant monitoring:** Optional, read-only MQTT Discovery with **21 entities** for sync progress, peers, storage, uptime, traffic and health indicators; scheduled updates via systemd timer.
- **Bandwidth management:** Optional upload/download limiting for the Bitcoin container, without shaping unrelated host services.
- **Operational visibility:** CLI helpers for synchronization status, block height and peer connections.
- **Maintainability:** Storage preflight checks, setup documentation and GitHub Actions covering Bash syntax, ShellCheck and Docker Compose validation.

**Validation:** Built and tested on Raspberry Pi 5 with Debian 13 and Bitcoin Core 31.1. The MQTT feature and documentation were merged in [PR #5](https://github.com/ChristophKomenda/bitcoin-pi-node/pull/5) and [PR #6](https://github.com/ChristophKomenda/bitcoin-pi-node/pull/6). Full initial synchronization and controlled restart testing are not yet documented as complete.

**Impact:** Making self-hosted Bitcoin infrastructure more approachable through reproducible deployment, safer storage handling and clear operational documentation.

[**Explore Bitcoin Pi Node →**](https://github.com/ChristophKomenda/bitcoin-pi-node) · [Home Assistant setup](https://github.com/ChristophKomenda/bitcoin-pi-node/blob/main/docs/home-assistant.md) · [MQTT monitoring PR](https://github.com/ChristophKomenda/bitcoin-pi-node/pull/5)

---

## How I Work

**Understand the user → design the experience → build the solution → measure and improve.**

I combine qualitative UX thinking with implementation and analytics. Depending on the project, that means improving task flows and interface clarity, writing HTML/CSS/JavaScript, working with WordPress and WooCommerce, auditing Core Web Vitals, or using GA4 events to understand how people interact with a site.

My open-source contributions follow a similar process: **investigate the problem, validate assumptions, implement a solution, test it and document the results.**

**My focus:** Meaningful outcomes, maintainable implementation and measurable impact. I prefer documented before-and-after evidence over unsupported performance or conversion claims. I also distinguish **tested**, **experimental** and **proposed** functionality when publishing open-source work.

## Skills & Technologies

| Area | Tools and capabilities |
| --- | --- |
| **UX/UI & Product Design** | Figma, Adobe Creative Cloud, responsive design, user journeys, information architecture, prototyping |
| **Frontend** | HTML, CSS, JavaScript, React, accessible and responsive interfaces |
| **E-Commerce & CMS** | WordPress, Elementor, WooCommerce, Shopify, Salesforce Commerce Cloud |
| **SEO & Optimization** | Technical SEO, Schema.org, Core Web Vitals, PageSpeed, conversion rate optimization (CRO) |
| **Analytics** | Google Analytics 4, Google Tag Manager, event tracking and performance analysis |
| **Software Development & Testing** | Python, API integration, protocol analysis, automated regression testing, Git, GitHub |
| **Infrastructure & Open Source** | Linux, Docker, Raspberry Pi, Home Assistant, REST APIs, Nginx, Cloudflare |

## Background

My professional background spans **UX/UI design, e-commerce, digital marketing and frontend development**, supported by training in business and IT and continued professional development in UX design, frontend technologies and digital product delivery.

I enjoy working at the intersection of **design, technology and business outcomes** — both in client-facing projects and in open-source communities.

[**See my experience and qualifications →**](https://christophkomenda.de/wp-content/uploads/2026/10/CV_Christoph_Komenda.pdf)

## More Projects

- [Sabine Hett](https://sabinehett.de) — local SEO, structured data and UX improvements
- [Physio-Aktiv](https://physio-aktiv-ck.de) — digital presence for physiotherapy and health services
- [Business Power Netzwerk](https://businesspowernetzwerk.de) — business website and digital presence
- [Digital CFO](https://www.digital-cfo.eu) — business website and digital presence
- [React frontend capstone](https://github.com/ChristophKomenda/final_project) — component-based React project
- [Christoph Komenda Design](https://christophkomenda.de) — portfolio and independent digital design work

---

## Let's Build Something Useful

I'm open to **UX/UI, frontend and e-commerce opportunities**, **selected freelance collaborations**, and **open-source contributions**.

If you're building a product, improving a digital customer journey or working on a project where design and engineering meet, I'd be happy to connect.

[**Explore my portfolio**](https://christophkomenda.de) · [**View my CV**](https://christophkomenda.de/wp-content/uploads/2026/10/CV_Christoph_Komenda.pdf) · [**Start a GitHub discussion**](https://github.com/ChristophKomenda/pironman5-homeassistant-container/discussions)

*Design thoughtfully. Build practically. Improve continuously.*
