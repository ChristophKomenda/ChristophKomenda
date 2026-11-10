# Hi, I'm Christoph Komenda

**UX/UI Designer · Frontend Developer · E-Commerce & Open Source**

I design and build intuitive digital experiences, connecting **user-centered design, frontend engineering, e-commerce and measurable optimization**.

From conversion-focused customer journeys to locally integrated smart-home software, I enjoy turning complex requirements into clear, practical solutions.

[**Portfolio**](https://christophkomenda.de) · [**Resume / CV**](https://christophkomenda.de/wp-content/uploads/2026/10/CV_Christoph_Komenda.pdf) · [**Explore my repositories**](https://github.com/ChristophKomenda?tab=repositories)

---

## Selected work

### Pironman 5 / 5 Max — Home Assistant Integration

**Open Source · Python · Home Assistant · HACS · REST API · Docker · Raspberry Pi**

Designed, developed, and maintain an open-source Home Assistant integration that enables **native monitoring and hardware control for SunFounder Pironman 5 / 5 Max** devices.

Built with **Home Assistant Container (Docker)** in mind, the integration bridges the gap between SunFounder's local hardware API and Home Assistant's native entities — without additional cloud services, MQTT, or a separate Home Assistant add-on.

**🏆 Key milestone: Official HACS acceptance**

Successfully reviewed, approved, and merged into the **HACS default repository**, allowing users to discover, install, and update the integration directly through HACS.

**Key engineering contributions**

- **Native hardware integration:** CPU, GPU, memory, NVMe storage, network monitoring, and cooling status.
- **Advanced device controls:** Fan profiles, RGB lighting effects, brightness, colors, and OLED display settings.
- **Container-first architecture:** Works with Home Assistant Container and supports network-based communication across separate devices.
- **Configurable REST API:** Adjustable host, port, and polling interval with fully local communication.
- **Open-source quality:** GitHub Actions validation, versioned releases, contribution guidelines, security documentation, and structured issue templates.
- **Hardware compatibility:** Published a model-specific compatibility matrix and reproducible testing plan, clearly distinguishing verified and untested hardware.

**Verified environment:** Pironman 5 Max with Home Assistant Container. Pironman 5 is a target model; additional Pironman variants require hardware validation.

**Impact:** Expanded Home Assistant integration options for Pironman users, especially those running Docker-based installations, and established a maintainable foundation for future hardware support and community contributions.

[**Explore project & installation →**](https://github.com/ChristophKomenda/pironman5-homeassistant-container) · [HACS acceptance](https://github.com/hacs/default/pull/12242) · [Hardware compatibility & testing](https://github.com/ChristophKomenda/pironman5-homeassistant-container/blob/main/docs/hardware-testing.md) · [Latest release](https://github.com/ChristophKomenda/pironman5-homeassistant-container/releases/latest)

### Weishaupt WTC — Protocol Reverse Engineering & Home Assistant Contributions

**Open Source · Python · Reverse Engineering · CanApiJson · Home Assistant · Hardware Validation · Automated Testing**

Investigating the local **Weishaupt WEM / CanApiJson protocol** to make heating-system data more accessible in Home Assistant. On a **WTC-GW 15-B**, I researched **12 heating-circuit (HK1) settings** and **13 additional WTC sensor registers**, documenting observed behavior, decoding requirements and validation limits.

The research has led to **10 pull requests across 3 upstream projects**, contributing read-only sensors, protocol handling, tests and documentation. **All 10 PRs remain open for upstream review as of November 10, 2026; these changes are not claimed as upstream releases.**

**🔬 Key engineering contributions**

- **HK1 heating-circuit monitoring:** Researched heating curve slope and parallel shift, minimum/maximum flow-temperature targets, summer/winter switching, frost protection and other configuration and efficiency-related parameters. A-B-A controller tests and live Home Assistant comparisons helped validate selected mappings.
- **13 additional WTC sensors — [PR #14](https://github.com/JS-DE-Tech/hacs-weishaupt-lan/pull/14):** Proposed read-only monitoring for burner and blower behavior, internal pump electrical power, pump limits and other boiler-related values. All 13 register addresses returned numeric replies in individual hardware probes; some meanings and units remain provisional.
- **Protocol edge cases:** Added support for separate GET request and response sizes, including HK1 registers that require **request VS=1 / response VS=2**, and a WTC pump-power register using **request VS=2 / response VS=1**.
- **Coordinator and polling improvements:** Proposed integrating the 13 WTC sensors into the regular Home Assistant coordinator rather than a separate research-only polling path, with a configurable **60-second default scan interval**. Existing saved intervals require manual adjustment.
- **Regression testing and reproducibility:** Added tests for register mapping, signed decoding, scaling, device assignment, stable entity IDs and polling behavior, plus read-only probe scripts and hardware observation logs. **100 local unit tests passed on the latest PR #14 head** (`30224e7`).
- **Safety and compatibility:** Kept additions read-only, preserved Home Assistant entity IDs, avoided unverified controller write commands and documented what has — and has not — been validated.

**Selected hardware observations**

| Area | Register(s) | Observed result |
|---|---|---|
| HK1 heating curve slope / parallel shift | `0x254B` / `0x25AD` | Controller-matched readings with × 0.1 decoding |
| HK1 minimum / maximum flow target | `0x251B` / `0x251C` | 15.0 °C / 80.0 °C; GET VS=1, reply VS=2 |
| HK1 summer/winter switching | `0x257B` | 16.0 °C; GET VS=1, reply VS=2 |
| WTC internal pump electrical power | `09/01/261B/02` | 11 W shown in Home Assistant and on the controller |
| WTC heating-pump limits | `07/00/256B/02` / `07/00/256C/02` | 30% / 80%, matching the controller settings |
| WTC burner target / blower control | `07/00/2542/00` / `07/00/257E/00` | Repeated, display-compared observations of 15.69% and ~10.4% respectively |

**Upstream contributions — awaiting review**

| Project | Pull requests | Scope |
|---|---|---|
| [JS-DE-Tech/hacs-weishaupt-lan](https://github.com/JS-DE-Tech/hacs-weishaupt-lan) | [#9](https://github.com/JS-DE-Tech/hacs-weishaupt-lan/pull/9) · [#10](https://github.com/JS-DE-Tech/hacs-weishaupt-lan/pull/10) · [#11](https://github.com/JS-DE-Tech/hacs-weishaupt-lan/pull/11) · [#12](https://github.com/JS-DE-Tech/hacs-weishaupt-lan/pull/12) · [#13](https://github.com/JS-DE-Tech/hacs-weishaupt-lan/pull/13) · **[#14](https://github.com/JS-DE-Tech/hacs-weishaupt-lan/pull/14)** | HK1 sensors, WTC sensor expansion, request-size handling and regular polling |
| [kraiz/hassio-weishaupt](https://github.com/kraiz/hassio-weishaupt) | [#21](https://github.com/kraiz/hassio-weishaupt/pull/21) · [#22](https://github.com/kraiz/hassio-weishaupt/pull/22) | Heating-curve sensors and 10 further read-only HK1 settings |
| [BorgNumberOne/Weishaupt_CanApiJson](https://github.com/BorgNumberOne/Weishaupt_CanApiJson) | [#9](https://github.com/BorgNumberOne/Weishaupt_CanApiJson/pull/9) · [#10](https://github.com/BorgNumberOne/Weishaupt_CanApiJson/pull/10) | Protocol register documentation and controller-based evidence |

**Validation status (November 10, 2026):** Hardware observations come from **one WTC-GW 15-B installation**. All 13 new WTC registers responded to standalone read-only probes, but not every physical meaning, enum or scale is fully controller-verified. Earlier polling runs experienced partial failed read batches and intermittent unavailable states; **long-duration stability with all 13 registers in regular 60-second polling remains unproven**. Compatibility with other models and firmware also remains unverified. PR #14 overlaps earlier HK1 changes in #9–#13 and may require rebasing after upstream review.

**Impact:** Turning undocumented controller behavior into reviewable, reproducible community contributions — creating a stronger foundation for transparent heating monitoring and data-driven optimization without changing heating settings.

[**Browse my Weishaupt pull requests →**](https://github.com/pulls?q=is%3Apr+author%3AChristophKomenda+weishaupt) · [WTC sensor expansion (PR #14)](https://github.com/JS-DE-Tech/hacs-weishaupt-lan/pull/14) · [Hardware observation log](https://github.com/ChristophKomenda/hacs-weishaupt-lan/blob/feat/wtc-13-candidates-sammelpr/docs/wtc-gw15b-canapijson-observations-2026-11-10.md)

### DNATest.ch — UX/UI & e-commerce relaunch

**UX/UI · WordPress · WooCommerce · HTML · CSS · JavaScript · SEO · CRO**

Redesigned and optimized a Swiss DNA-testing e-commerce experience, focusing on clarity, trust, accessibility of product information and the path from discovery to purchase.

- Reworked content hierarchy, navigation, product presentation and calls to action
- Improved responsive layouts and reusable frontend components
- Implemented structured data and technical SEO enhancements
- Focused on page performance, usability and conversion-oriented journeys

[**Explore DNATest.ch**](https://dnatest.ch)

### SR Brennholzhandel — Local business website optimization

**Web design · WordPress · Frontend · Local SEO · GA4 · CRO**

Built and optimized a regional firewood supplier's digital presence to make products, delivery details and contact options easier to understand and act on.

- Improved information architecture and mobile user journeys
- Introduced prominent contact options and conversion-focused calls to action
- Implemented structured data and analytics event tracking
- Worked on frontend performance and technical SEO

[**Visit SR Brennholzhandel**](https://sr-brennholz.de)

### SunFounder — Upstream contributions

**Open-source collaboration · Raspberry Pi · Linux · Compatibility**

Contributed fixes and platform compatibility updates to SunFounder's upstream projects:

- [OLED / SSD1306 font asset path fix](https://github.com/sunfounder/pm_auto/pull/19) — corrected an asset path issue in the upstream driver
- [Debian Trixie compatibility contribution](https://github.com/sunfounder/pironman5/pull/109) — contributed tested platform compatibility information

These contributions complement my independent Home Assistant integration work and reflect a focus on maintainable, useful improvements.

---

## How I work

**Understand the user → design the experience → build the solution → measure and improve.**

I combine qualitative UX thinking with implementation and analytics. Depending on the project, that means improving task flows and interface clarity, writing HTML/CSS/JavaScript, working with WordPress and WooCommerce, auditing Core Web Vitals, or using GA4 events to understand how people interact with a site.

My open-source contributions follow a similar process: **investigate the problem, validate assumptions, implement a solution, test it and document the results.**

**My focus:** meaningful outcomes, maintainable implementation and measurable impact. I prefer documented before-and-after evidence over unsupported performance or conversion claims.

## Skills & technologies

| Area | Tools and capabilities |
|---|---|
| **UX/UI & product design** | Figma, Adobe Creative Cloud, responsive design, user journeys, information architecture, prototyping |
| **Frontend** | HTML, CSS, JavaScript, React, accessible and responsive interfaces |
| **E-commerce & CMS** | WordPress, Elementor, WooCommerce, Shopify, Salesforce Commerce Cloud |
| **SEO & optimization** | Technical SEO, Schema.org, Core Web Vitals, PageSpeed, conversion rate optimization (CRO) |
| **Analytics** | Google Analytics 4, Google Tag Manager, event tracking and performance analysis |
| **Software development & testing** | Python, API integration, protocol analysis, automated regression testing, Git, GitHub |
| **Infrastructure & open source** | Linux, Docker, Raspberry Pi, Home Assistant, REST APIs, Nginx, Cloudflare |

## Background

My professional background spans **UX/UI design, e-commerce, digital marketing and frontend development**, supported by training in business and IT and continued professional development in UX design, frontend technologies and digital product delivery.

I enjoy working at the intersection of **design, technology and business outcomes** — both in client-facing projects and in open-source communities.

[**See my experience and qualifications**](https://christophkomenda.de/wp-content/uploads/2026/10/CV_Christoph_Komenda.pdf)

## More projects

- [Sabine Hett](https://sabinehett.de) — local SEO, structured data and UX improvements
- [Physio-Aktiv](https://physio-aktiv-ck.de) — digital presence for physiotherapy and health services
- [Business Power Netzwerk](https://businesspowernetzwerk.de) — business website and digital presence
- [Digital CFO](https://www.digital-cfo.eu) — business website and digital presence
- [React frontend capstone](https://github.com/ChristophKomenda/final_project) — component-based React project
- [Christoph Komenda Design](https://christophkomenda.de) — portfolio and independent digital design work

---

## Let's build something useful

I'm open to **UX/UI, frontend and e-commerce opportunities**, **selected freelance collaborations**, and **open-source contributions**.

If you're building a product, improving a digital customer journey or working on a project where design and engineering meet, I'd be happy to connect.

**[Explore my portfolio](https://christophkomenda.de)** · **[View my CV](https://christophkomenda.de/wp-content/uploads/2026/10/CV_Christoph_Komenda.pdf)** · **[Start a GitHub discussion](https://github.com/ChristophKomenda/pironman5-homeassistant-container/discussions)**

*Design thoughtfully. Build practically. Improve continuously.*
