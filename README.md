
# Hi, I'm Christoph Komenda

**UX/UI Designer · Frontend Developer · Digital Products · E-Commerce & Open Source**

I design and build **user-centered digital products that solve real-world problems** — from complex e-commerce journeys to local-first IoT integrations.

My work connects UX/UI, frontend engineering, e-commerce, product thinking and measurable outcomes. I help businesses make digital customer journeys easier to navigate and build open-source software that makes hardware easier to use, monitor and maintain.

[**View my CV**](https://christophkomenda.de/wp-content/uploads/2026/10/CV_Christoph_Komenda.pdf) · [**Explore my portfolio**](https://christophkomenda.de) · [**Get in touch**](#lets-build-something-useful) · [Open-source repositories](https://github.com/ChristophKomenda?tab=repositories)

**Open to opportunities in UX/UI, frontend engineering, e-commerce and digital product teams, including roles at the intersection of design and technology.**

## Start here

| For you | Explore |
| --- | --- |
| **Recruiters & hiring managers** | [Experience](#background) · [Skills](#skills--technologies) · [CV](https://christophkomenda.de/wp-content/uploads/2026/10/CV_Christoph_Komenda.pdf) |
| **Product & e-commerce teams** | [Client projects](#dnatestch--uxui--e-commerce-relaunch) · [How I work](#how-i-work) |
| **Engineers & maintainers** | [Pironman integration](#pironman-5--5-max--home-assistant-integration) · [Upstream contributions](#weishaupt-wtc--protocol-reverse-engineering--upstream-contributions) |

## Real-world problems. Practical solutions.

| User need | My contribution & evidence |
| --- | --- |
| **Make complex purchasing decisions easier** | [DNATest.ch](#dnatestch--uxui--e-commerce-relaunch) — clearer product information, navigation and conversion-oriented journeys |
| **Make hardware easier to install and use** | [Pironman](#pironman-5--5-max--home-assistant-integration) — HACS default acceptance and independently tested HAOS installation improvements; [SunFounder community listing](https://github.com/sunfounder/home-assistant-addon/pull/27) |
| **Understand heating-system behavior** | [Weishaupt](#weishaupt-wtc--protocol-reverse-engineering--upstream-contributions) — 24 read-only sensors across three merged upstream PRs |
| **Diagnose intermittent battery communication failures** | [hm2mqtt](#hm2mqtt--battery-communication-diagnostics) — five proposed diagnostic entities, 40 additional unit tests and natural recovery observed on hardware; [open PR #490](https://github.com/tomquist/hm2mqtt/pull/490) |
| **Make Bluetooth devices easier to configure and integrate** | [Sendspin](#sendspin-bluetooth-bridge--ux--hardware-performance) — configuration UX and hardware-validated adapter resolution; [Apple BLE](#habluetooth--apple-ble--native-bluetooth-reception) — proposed optional native Bluetooth reception |
| **Improve heating setpoint precision** | [Tado Hijack](#tado-hijack--climate-control--upstream-contribution) — temperature-step correction implemented upstream in dev.17 |

*Evidence matters: I distinguish merged contributions, hardware-tested implementations and proposals still under review.*

<!-- Profile UX refresh: audience navigation and verified milestones (2026-11-25) -->

<details>
<summary><strong>More verified milestones & engineering evidence</strong></summary>

### Selected milestones

| Evidence | What it demonstrates |
| --- | --- |
| [**HACS default repository acceptance**](https://github.com/hacs/default/pull/12242) | Independently developed integration available through HACS discovery and updates |
| [**SunFounder community listing — merged PR #27**](https://github.com/sunfounder/home-assistant-addon/pull/27) | Manufacturer documentation recognition following independent HAOS testing and installation UX improvements (November 24, 2026) |
| [**Weishaupt upstream contributions**](https://github.com/kraiz/hassio-weishaupt/pulls?q=is%3Apr+author%3AChristophKomenda) | Three merged contributions adding 24 read-only sensors |
| **Inkcut upstream contributions** — [#450](https://github.com/inkcut/inkcut/pull/450) · [#451](https://github.com/inkcut/inkcut/pull/451) | Two upstream proposals for network serial transport and native device support; physical pen-plot validation |
| **Energy monitoring & MQTT security** — [hm2mqtt #490](https://github.com/tomquist/hm2mqtt/pull/490) · [GroBro #244–#247](https://github.com/robertzaage/GroBro/pulls?q=is%3Apr+author%3AChristophKomenda) | Proposed communication diagnostics and secure MQTT deployment improvements, supported by automated tests, ARM64 deployment observations and benchmarks |
| [**Tado Hijack #217**](https://github.com/banter240/tado_hijack/pull/217) | Temperature-step correction implemented upstream in dev.17, as confirmed by the maintainer |
| **Sendspin Bluetooth Bridge** — [#605](https://github.com/trudenboy/sendspin-bt-bridge/pull/605) · [#606](https://github.com/trudenboy/sendspin-bt-bridge/pull/606) | Two open proposals addressing configuration UX and Bluetooth controller resolution, with focused tests and real-hardware benchmarks |
| **Native Apple BLE reception** — [habluetooth #662](https://github.com/Bluetooth-Devices/habluetooth/pull/662) · [Apple BLE #6](https://github.com/hudsonbrendon/ha-apple-ble/pull/6) | Coordinated API and integration proposals, validated with local and remote Bluetooth reception |

*The SunFounder IR add-on remains community-maintained, not officially supported by the manufacturer.*

**Find what matters to you:**

- [Client projects](#dnatestch--uxui--e-commerce-relaunch) — UX, e-commerce and digital experiences
- [Hiring & qualifications](#background) — experience, skills and professional background
- [Open-source engineering](#pironman-5--5-max--home-assistant-integration) — software, hardware and upstream contributions

### At a glance

I work across **UX/UI, frontend and e-commerce**, and contribute to open-source projects that turn real hardware and protocol research into maintainable software.

| Focus | Evidence | Explore |
| --- | --- | --- |
| **UX & e-commerce** | Customer journeys, product presentation, SEO and conversion-oriented frontend work | [DNATest.ch](#dnatestch--uxui--e-commerce-relaunch) · [SR Brennholzhandel](#sr-brennholzhandel--local-business-website-optimization) |
| **Home Assistant & Python** | Pironman 5 integration accepted into **HACS default**; IR add-on listed in **SunFounder's official documentation** | [Pironman 5](#pironman-5--5-max--home-assistant-integration) · [SunFounder](#sunfounder--upstream-contributions) |
| **Protocol engineering** | **3 merged upstream PRs** adding **24 read-only Weishaupt sensors** | [Weishaupt WTC](#weishaupt-wtc--protocol-reverse-engineering--upstream-contributions) |
| **Network serial & hardware integration** | RFC2217 transport prototype, six new regression tests and physical SVG pen plotting | [Inkcut](#inkcut--network-serial-transport--plotter-integration) |
| **Energy monitoring & secure IoT** | Five proposed battery communication diagnostics, 991 passing unit tests in hm2mqtt validation and four GroBro proposals covering TLS security and deployment | [hm2mqtt](#hm2mqtt--battery-communication-diagnostics) · [GroBro](#grobro--secure-mqtt--solar-infrastructure) |
| **Network monitoring & MQTT** | Powerline2MQTT: three adapters and **31 validated Home Assistant entities** | [Powerline2MQTT](#powerline2mqtt--local-powerline-network-monitoring) |
| **Release engineering & developer experience** | Three HAOS app packages, automated upstream synchronization, SHA-256 integrity checks and five native architecture build targets | [Community Apps](#home-assistant-community-apps--automated-app-distribution) · [Bitcoin Node Monitor](#bitcoin-node-monitor--local-bitcoin-core-monitoring) |
| **Self-hosted infrastructure** | Bitcoin Pi Node with guarded storage startup and **21 optional MQTT entities** | [Bitcoin Pi Node](#bitcoin-pi-node--secure-self-hosted-bitcoin-core) |
| **Bluetooth & system integration** | Native BLE callback proposals, real AirPods reception, Bluetooth controller diagnostics and bounded performance caching | [Sendspin](#sendspin-bluetooth-bridge--ux--hardware-performance) · [Apple BLE](#habluetooth--apple-ble--native-bluetooth-reception) |

**For hiring and collaboration:** [Experience & qualifications](#background) · [Skills](#skills--technologies) · [How I work](#how-i-work) · [Get in touch](#lets-build-something-useful)

**Explore selected work:** [Sendspin](#sendspin-bluetooth-bridge--ux--hardware-performance) · [Apple BLE](#habluetooth--apple-ble--native-bluetooth-reception) · [Tado Hijack](#tado-hijack--climate-control--upstream-contribution) · [hm2mqtt](#hm2mqtt--battery-communication-diagnostics) · [GroBro](#grobro--secure-mqtt--solar-infrastructure) · [Inkcut](#inkcut--network-serial-transport--plotter-integration) · [Pironman 5](#pironman-5--5-max--home-assistant-integration) · [Weishaupt WTC](#weishaupt-wtc--protocol-reverse-engineering--upstream-contributions) · [E-Commerce](#dnatestch--uxui--e-commerce-relaunch) · [SunFounder IR](#sunfounder--upstream-contributions) · [Powerline2MQTT](#powerline2mqtt--local-powerline-network-monitoring) · [Bitcoin Pi Node](#bitcoin-pi-node--secure-self-hosted-bitcoin-core) · [Community Apps](#home-assistant-community-apps--automated-app-distribution) · [Bitcoin Node Monitor](#bitcoin-node-monitor--local-bitcoin-core-monitoring)

</details>

---

## Selected work

*Selected projects, outcomes and evidence. Expand technical sections when you want more detail.*

### DNATest.ch — UX/UI & E-Commerce Relaunch

**Focus: Making complex product decisions clearer and easier to navigate.**

**UX/UI · WordPress · WooCommerce · HTML · CSS · JavaScript · SEO · CRO**

Redesigned and optimized a Swiss DNA-testing e-commerce experience, focusing on clarity, trust, accessibility of product information and the path from discovery to purchase.

- Reworked content hierarchy, navigation, product presentation and calls to action
- Improved responsive layouts and reusable frontend components
- Implemented structured data and technical SEO enhancements
- Focused on page performance, usability and conversion-oriented journeys

[**Explore DNATest.ch →**](https://dnatest.ch)

### SR Brennholzhandel — Local Business Website Optimization

**Focus: Helping local customers find products, delivery information and contact options quickly.**

**Web Design · WordPress · Frontend · Local SEO · GA4 · CRO**

Built and optimized a regional firewood supplier's digital presence to make products, delivery details and contact options easier to understand and act on.

- Improved information architecture and mobile user journeys
- Introduced prominent contact options and conversion-focused calls to action
- Implemented structured data and analytics event tracking
- Worked on frontend performance and technical SEO

[**Visit SR Brennholzhandel →**](https://sr-brennholz.de)

### Pironman 5 / 5 Max — Home Assistant Integration

**Open Source · Python · Home Assistant · HACS · REST API · Docker · Raspberry Pi**

Designed, developed, and maintain an open-source Home Assistant integration that enables **native monitoring and hardware control for SunFounder Pironman 5 / 5 Max** devices.

Built with **Home Assistant Container (Docker)** in mind, the integration bridges the gap between SunFounder's local hardware API and Home Assistant's native entities — without additional cloud services, MQTT, or a separate Home Assistant add-on for core functionality.

**🏆 Key milestones**

| Milestone | Outcome |
| --- | --- |
| **Official HACS acceptance** | Reviewed, approved and merged into the HACS default repository, enabling direct discovery, installation and updates. |
| **SunFounder documentation listing** | The community-maintained Pironman 5 Max IR receiver add-on is now listed in SunFounder's official Home Assistant add-on repository following the merge of [PR #27](https://github.com/sunfounder/home-assistant-addon/pull/27) on November 24, 2026. |

**Recent milestone: v1.5.0 — experimental native IR / HAIR receiver support**

The integration now includes an optional native Home Assistant infrared receiver for the **Pironman 5 Max**, connected via a separately installed Linux/LIRC host bridge.

It was tested with HAIR on real hardware; the IR capability remains experimental, receive-only and disabled by default.

Version 1.4.0 also introduced expanded network and device diagnostics with capability-aware model detection, without claiming verified Pro Max support.

**Extended HAOS support**

A complementary, community-maintained IR receiver add-on extends the infrared functionality to Home Assistant OS users. Its v0.2.0 event-based architecture connects directly to the existing HACS integration, removing the need for manual installation of a separate companion integration.

<details>
<summary><strong>Explore Pironman engineering details (features, architecture, tests)</strong></summary>

**Key engineering contributions**

- **Native hardware integration:** CPU, GPU, memory, dynamically discovered NVMe / USB storage, network monitoring, and cooling status.
- **Advanced device controls:** Fan profiles, RGB lighting effects, brightness, colors, and OLED display settings.
- **Container-first architecture:** Works with Home Assistant Container and supports network-based communication across separate devices.
- **Configurable REST API:** Adjustable host, port, and polling interval with fully local communication.
- **Open-source quality:** GitHub Actions validation, versioned releases, contribution guidelines, security documentation, and structured issue templates.
- **Hardware compatibility:** Published a model-specific test matrix and capability-aware detection, distinguishing maintainer-tested Pironman 5 Max hardware from unverified models.
- **Optional infrared reception:** Home Assistant `InfraredReceiverEntity`, HAIR integration and a documented host-side LIRC bridge for Pironman 5 Max.
- **HAOS interoperability:** Complementary IR receiver add-on with event-based communication to the existing HACS integration.
- **Installation UX:** Removed the need to manually copy a separate companion integration into Home Assistant's configuration directory.
- **Maintainer collaboration:** Incorporated manufacturer feedback into the installation architecture and documentation.

</details>

**Verified environment:** Pironman 5 Max with Home Assistant Container. The companion IR add-on has also received independent community testing on Home Assistant OS. Pironman 5 is a target model; additional Pironman variants require hardware validation.

**Impact:** Expanded Home Assistant integration options for Pironman users across Container and HAOS environments, reduced installation friction, and established a maintainable foundation for future hardware support and community contributions.

[**Explore project & installation →**](https://github.com/ChristophKomenda/pironman5-homeassistant-container) · [IR / HAIR documentation](https://github.com/ChristophKomenda/pironman5-homeassistant-container/blob/main/docs/native-ir-hair.md) · [HACS acceptance](https://github.com/hacs/default/pull/12242) · [SunFounder community listing](https://github.com/sunfounder/home-assistant-addon/pull/27) · [Hardware compatibility & testing](https://github.com/ChristophKomenda/pironman5-homeassistant-container/blob/main/docs/hardware-testing.md) · [Latest release](https://github.com/ChristophKomenda/pironman5-homeassistant-container/releases/latest)

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

<details>
<summary><strong>Explore Weishaupt technical evidence, register mappings & upstream PR status</strong></summary>

**Key engineering contributions**

- **Heating-circuit monitoring:** Validated heating curve slope, parallel shift, minimum and maximum flow-temperature targets, summer/winter switching thresholds, frost protection and additional HK1 configuration parameters.
- **Protocol reverse engineering:** Identified undocumented CanApiJson register mappings and request/response behavior through direct hardware measurements.
- **Protocol compatibility:** Implemented independent request and response value sizes for selected registers while preserving existing sensor behavior.
- **Regression testing:** Added automated tests covering register addresses, scaling, signed decoding, response validation and backward compatibility.
- **Hardware validation:** Used repeated read-only probes, physical controller comparisons and controlled A-B-A measurements.
- **Boiler sensor expansion:** Added 12 WTC sensors upstream in [PR #24](https://github.com/kraiz/hassio-weishaupt/pull/24), covering burner modulation, blower operation, pump performance and diagnostic parameters.
- **Additional protocol research:** Proposed 13 WTC sensor candidates with regular 60-second polling in [JS-DE-Tech PR #14](https://github.com/JS-DE-Tech/hacs-weishaupt-lan/pull/14).
- **Device clock diagnostics:** Proposed timezone-aware device timestamps, signed clock drift diagnostics, DST handling and fresh-register validation without additional polling or write operations in [PR #18](https://github.com/JS-DE-Tech/hacs-weishaupt-lan/pull/18). The published proposal reports 76 passing tests; subsequent local production-patch validation reported 87 passing tests. Broader hardware validation remains outstanding.
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

**Upstream contribution snapshot — November 26, 2026**

| Project | Status | Contributions |
| --- | --- | --- |
| [kraiz/hassio-weishaupt](https://github.com/kraiz/hassio-weishaupt) | **3 merged** | [#21](https://github.com/kraiz/hassio-weishaupt/pull/21), [#22](https://github.com/kraiz/hassio-weishaupt/pull/22), [#24](https://github.com/kraiz/hassio-weishaupt/pull/24) |
| [JS-DE-Tech/hacs-weishaupt-lan](https://github.com/JS-DE-Tech/hacs-weishaupt-lan) | **7 open** | [#9–#14](https://github.com/JS-DE-Tech/hacs-weishaupt-lan/pulls?q=is%3Apr+author%3AChristophKomenda), [#18](https://github.com/JS-DE-Tech/hacs-weishaupt-lan/pull/18) |
| [BorgNumberOne/Weishaupt_CanApiJson](https://github.com/BorgNumberOne/Weishaupt_CanApiJson) | **2 open** | [#9](https://github.com/BorgNumberOne/Weishaupt_CanApiJson/pull/9), [#10](https://github.com/BorgNumberOne/Weishaupt_CanApiJson/pull/10) |

**Validation scope:** Research findings are based on one WTC-GW 15-B installation. Additional device models, firmware versions and provisional register interpretations require further validation. Long-term polling stability and live integration testing of the newly merged WTC sensors remain outstanding.

</details>

**Impact:** Transforming undocumented heating-controller behavior into tested, documented and upstream-accepted open-source functionality that other Home Assistant users and developers can build upon.

[**Merged upstream contributions →**](https://github.com/kraiz/hassio-weishaupt/pulls?q=is%3Apr+author%3AChristophKomenda) · [WTC sensor expansion](https://github.com/JS-DE-Tech/hacs-weishaupt-lan/pull/14) · [Hardware research](https://github.com/ChristophKomenda/hacs-weishaupt-lan/blob/feat/wtc-13-candidates-sammelpr/docs/wtc-gw15b-canapijson-observations-2026-11-10.md)

<!-- Energy and MQTT portfolio update: 2026-11-26 -->

### hm2mqtt — Battery Communication Diagnostics

**Open Source · TypeScript · Node.js · MQTT Discovery · Home Assistant · ARM64 · Observability**

Investigated 318 communication timeout warnings over ten days on a Marstek Jupiter C Plus installation and developed optional, read-only communication diagnostics to make device communication behavior observable directly in Home Assistant.

The proposed implementation introduces no additional hardware polling or device control commands and remains disabled by default.

**Engineering milestone: Five diagnostic entities and comprehensive automated validation**

| Validation | Result |
| --- | --- |
| Unit tests | **991 passed** |
| Additional unit tests | **40** |
| Unit test suites | 28 passed |
| Overall statement coverage | 91.59% |
| Automated review follow-up | All three initial findings addressed; no new actionable findings |
| Communication diagnostics coverage | 100% |
| Communication discovery coverage | 100% |
| Home Assistant E2E tests | 8 passed |
| Add-on configuration tests | 5 passed |
| Discovery baseline families | 20 |
| Discovery upgrade safety | Passed |
| Lint, formatting and build | Passed |

Six optional firmware-emulator tests were skipped.

<details>
<summary><strong>Explore hm2mqtt architecture, hardware validation & performance benchmarks</strong></summary>

**Key engineering contributions**

- **Problem investigation:** Analyzed recurring communication timeout warnings on a real Marstek Jupiter C Plus installation without claiming to have established their root cause.
- **Observability:** Introduced five diagnostic entities covering communication timeouts, consecutive timeouts, received device messages and timestamps of the latest message and timeout.
- **MQTT architecture:** Independent per-device statistics, retained state, retained discovery, reconnect support and discovery lifecycle management.
- **Backward compatibility:** Optional activation, disabled by default, without changing existing polling or device controls.
- **Home Assistant integration:** Add-on configuration support, English and German translations, and documentation.
- **Regression testing:** Expanded automated coverage and validated discovery upgrade safety.
- **Performance engineering:** Compared upstream, disabled and enabled configurations across two Node.js container environments.

**Initial real-hardware validation**

| Component | Environment |
| --- | --- |
| Hardware | Marstek Jupiter C Plus (JPLS-8H) |
| Firmware | 143.39.217.110 |
| Host | Raspberry Pi 5 / ARM64 |
| Deployment | Docker Compose |
| Smart home | Home Assistant Container |

During initial operation, all five diagnostic entities appeared under the existing Home Assistant device. The timeout counter matched observed warnings, and the consecutive timeout counter returned to zero after natural communication recovery.

**Initial memory benchmark**

18 benchmark runs using three simulated devices, two-second polling and 120-second measurement windows.

| Runtime | Upstream RSS | Diagnostics disabled | Diagnostics enabled |
| --- | --- | --- | --- |
| Node.js 24 Debian | 84.406 MiB | 86.078 MiB | 86.234 MiB |
| Node.js 26 Alpine | 78.250 MiB | 79.688 MiB | 80.031 MiB |

Observed median RSS overhead with diagnostics enabled was approximately **2.2%** compared with upstream.

**Validation scope:** Hardware observations and benchmarks refer to the initial implementation before the final discovery lifecycle improvements. Extended operation and final-revision validation remain outstanding. Short benchmarks do not establish long-term memory leak freedom. Received messages are not equivalent to successful request-response pairs.

</details>

**Status (November 26, 2026):** Open upstream PR, ready for maintainer review. All three initial CodeRabbit findings were addressed in [commit ae6d1a0](https://github.com/ChristophKomenda/hm2mqtt/commit/ae6d1a0); the follow-up automated review reported no new actionable findings and assessed merge risk as minimal. The 991 unit tests and eight E2E tests passed locally after the review fixes. This is not a maintainer approval or a merged feature; final hardware and benchmark validation remain outstanding.

**Expected impact:** Improved visibility into battery communication reliability, easier troubleshooting and more actionable local energy-system diagnostics without increasing hardware polling.

[**Explore upstream PR #490 →**](https://github.com/tomquist/hm2mqtt/pull/490)

### GroBro — Secure MQTT & Solar Infrastructure

**Open Source · Python · MQTT · TLS · PKI · Mosquitto · Docker Compose · Growatt · Raspberry Pi**

Developed four independent upstream proposals focused on secure MQTT communication, reproducible infrastructure deployment and improved developer experience for Growatt inverter integrations.

The work addresses authenticated MQTT communication, certificate lifecycle management, network troubleshooting and optional certificate and hostname verification.

| Upstream contribution | Focus |
| --- | --- |
| [**PR #244 — Authenticated deployment**](https://github.com/robertzaage/GroBro/pull/244) | Docker Compose deployment with authenticated source and target MQTT brokers |
| [**PR #245 — TLS certificate renewal**](https://github.com/robertzaage/GroBro/pull/245) | DNS-01 issuance, certificate renewal and Mosquitto reload documentation |
| [**PR #246 — Troubleshooting guide**](https://github.com/robertzaage/GroBro/pull/246) | MQTT connectivity, DNS, gateway visibility, authentication and discovery |
| [**PR #247 — TLS verification**](https://github.com/robertzaage/GroBro/pull/247) | Optional certificate and hostname verification with system or custom CA trust |

<details>
<summary><strong>Explore GroBro security architecture, testing & infrastructure</strong></summary>

**Key engineering contributions**

- **Secure MQTT infrastructure:** Dedicated TLS-enabled source broker and separate authenticated Home Assistant target broker.
- **Transport security:** Proposed explicit certificate and hostname verification using system trust stores or custom PEM CA bundles.
- **Independent configuration:** Separate security settings for source and target MQTT clients.
- **Fail-closed verification:** Invalid verification settings must not silently downgrade to insecure TLS.
- **Certificate lifecycle:** DNS-01 certificate issuance, renewal dry runs, certificate-chain inspection and broker reload procedures.
- **Backward compatibility:** Existing plaintext and legacy TLS defaults preserved; secure verification requires explicit activation.
- **Developer experience:** Reproducible deployment examples and structured troubleshooting documentation.
- **Automated testing:** Added regression tests for secure SSL contexts, custom CA handling, missing CA failures and independent broker configuration.

**Validation**

- Raspberry Pi 5 / ARM64 deployment observations.
- TLS broker handshakes and authenticated broker logins.
- DNS-01 certificate issuance and renewal dry run.
- Local Ruff and full pytest suite passed for the proposed TLS implementation.

**Validation scope:** Full end-to-end inverter telemetry, generalized deployment examples and complete runtime validation remain outstanding. The four contributions are upstream proposals, not claimed as merged or released.

</details>

**Expected impact:** More secure, maintainable and reproducible local solar-energy integrations, with clearer installation and troubleshooting workflows.

[**Explore GroBro contributions →**](https://github.com/robertzaage/GroBro/pulls?q=is%3Apr+author%3AChristophKomenda)

### Tado Hijack — Climate Control & Upstream Contribution

**Open Source · Python · Home Assistant · Tado X · API Debugging · Regression Testing**

Investigated a temperature-setting issue in Tado Hijack v5.13.0 using a Home Assistant Container installation with 11 Tado X heating zones. A requested setpoint of 19.5 °C was rounded to 20 °C in the outgoing Hops API payload.

<details>
<summary><strong>Explore the proposed fix & validation</strong></summary>

- **Root cause analysis:** Traced the behavior to unconditional integer rounding in the climate entity.
- **API debugging:** Identified discrepancies between requested temperature setpoints and outgoing Hops API payloads.
- **Precision-aware implementation:** Proposed respecting the advertised target temperature step while preserving backward compatibility.
- **Regression testing:** Added isolated tests for fractional and integer temperature steps, missing temperature input and coordinator payload handling.
- **Code quality:** Ran targeted regression tests and Ruff lint locally.

</details>

**Upstream milestone — implemented in dev.17:** The maintainer confirmed implementation of the reported temperature-step correction on November 26, 2026, following [PR #217](https://github.com/banter240/tado_hijack/pull/217). The PR was closed rather than directly merged. Live hardware validation of the upstream implementation remains outstanding.

**Intended impact:** More predictable temperature control and alignment between the Home Assistant interface and the values sent to the heating system.

[**Explore upstream contribution →**](https://github.com/banter240/tado_hijack/pull/217)


<!-- Bluetooth engineering update: 2026-11-26 -->

### Sendspin Bluetooth Bridge — UX & Hardware Performance

**Open Source · JavaScript · Python · Bluetooth · BlueZ · D-Bus · Linux · Docker · Performance Engineering**

Investigated two independent issues while deploying a local Bluetooth audio endpoint for Music Assistant on Raspberry Pi 5.

The resulting upstream contributions address both configuration UX and Bluetooth controller identity resolution.

| Contribution | Outcome |
| --- | --- |
| [PR #605 — Manual device registration](https://github.com/trudenboy/sendspin-bt-bridge/pull/605) | Prevents delegated click-event arguments from incorrectly populating the Bluetooth MAC address field. |
| [PR #606 — Default adapter resolution](https://github.com/trudenboy/sendspin-bt-bridge/pull/606) | Resolves the actual default Bluetooth controller and introduces bounded caching to reduce repeated synchronous hardware queries. |

<details>
<summary><strong>Explore Sendspin root cause analysis, regression tests & performance benchmarks</strong></summary>

**Frontend and configuration UX — PR #605**

- Reproduced an invalid `[object PointerEvent]` value in the MAC address input during manual device registration.
- Traced the issue to argument forwarding in the delegated JavaScript action dispatcher.
- Introduced a narrowly scoped action wrapper that preserves explicit device-registration calls.
- Added a focused automated regression test and validated JavaScript syntax.

**Bluetooth controller identity — PR #606**

- Reproduced an unresolved default HCI identity despite an available Bluetooth controller.
- Mapped the actual BlueZ controller MAC address to its kernel HCI identity.
- Preserved explicit adapter configuration and default command scope.
- Avoided assuming that the default controller is always `hci0`.
- Introduced a five-second successful-resolution cache and a one-second failed-resolution cache.
- Added 12 focused regression tests covering controller changes, missing mappings, delayed availability and cache behavior.

**Measured performance on Raspberry Pi 5**

| Scenario | Measured time |
| --- | ---: |
| Uncached dynamic resolution — median | 11.255 ms |
| Cold cached implementation | 14.001 ms |
| Warm cache — median of 1,000 lookups | 0.000370 ms |
| Warm cache — maximum | 0.004204 ms |
| Refresh after cache expiration | 15.570 ms |

The warm-cache median was approximately **30,400 times lower** than the previously measured uncached median. This is a microbenchmark of adapter lookups, not an overall application speedup.

**Hardware validation**

- Raspberry Pi 5 / ARM64, Debian 13, Linux 6.18.60 and BlueZ 5.82.
- Sendspin Bluetooth Bridge v2.76.6 and Music Assistant 2.10.9.
- Wavemaster CUBE MINI Bluetooth speaker.
- Concurrent ESPHome-compatible Bluetooth proxy operation.
- Successful resolution of the real controller and its D-Bus device path.
- Active Bluetooth playback before and after the isolated test.
- No production container restarts or installed application-file changes.
- All 12 focused adapter regression tests passed; Ruff and formatting checks passed.

</details>

**Status:** Both upstream PRs are open and submitted for review as of November 26, 2026.

**Validation scope:** The actual patched adapter module was tested in a separate process within the installed v2.76.6 container. Full current-main CI, concurrent cache access and end-to-end AVRCP validation remain outstanding. Full browser UI validation of PR #605 is also pending.

**Impact:** Reduces Bluetooth configuration friction and proposes a more reliable, efficient controller identity resolution mechanism.

[**Frontend contribution #605**](https://github.com/trudenboy/sendspin-bt-bridge/pull/605) · [**Bluetooth contribution #606**](https://github.com/trudenboy/sendspin-bt-bridge/pull/606)


### habluetooth & Apple BLE — Native Bluetooth Reception

**Open Source · Python · Cython · Bluetooth Low Energy · Home Assistant · BlueZ · API Design · ARM64**

Developed two coordinated upstream proposals to enable optional native reception of Apple proximity-pairing advertisements in Home Assistant.

The architecture preserves the existing Bluetooth noise-filtering behavior while offering interested integrations an explicit opt-in mechanism.

| Project | Contribution |
| --- | --- |
| [habluetooth PR #662](https://github.com/Bluetooth-Devices/habluetooth/pull/662) | Proposed an opt-in callback API for selected filtered Apple advertisements. |
| [Apple BLE PR #6](https://github.com/hudsonbrendon/ha-apple-ble/pull/6) | Proposed native advertisement reception through the optional habluetooth API, retaining compatibility with existing ESPHome-based reception. |

<details>
<summary><strong>Explore Bluetooth architecture, compatibility & hardware validation</strong></summary>

**Bluetooth manager API**

- Preserved the existing Apple advertisement pre-filter and normal discovery behavior.
- Introduced optional subscriptions for matching filtered Apple advertisements.
- Supported independent subscriptions and idempotent cancellation.
- Isolated subscriber exceptions.
- Preserved existing advertisement history and per-address callbacks.
- Synchronized Python and Cython declarations without introducing additional runtime dependencies.

**Integration compatibility**

- Retained normal Home Assistant Bluetooth callbacks.
- Used capability detection for the proposed optional native API.
- Preserved the existing ESPHome tap when the optional API is unavailable.
- Avoided automatic installation of a patched dependency.

**Automated validation**

| Test environment | Result |
| --- | --- |
| Patched habluetooth 7.1.2 | 46 tests passed; 97% reported coverage |
| Standard habluetooth 7.1.3 | 46 tests passed; 97% reported coverage |
| Native callback helper | 100% statement coverage |
| Additional isolated tests | 22 |

**Physical hardware validation**

- Home Assistant Container 2026.11.1 on Raspberry Pi 5 / ARM64.
- Python 3.14.10 and BlueZ 5.82.
- Apple AirPods (2nd generation).
- Native local Bluetooth reception.
- Remote Raspberry Pi ESPHome-compatible Bluetooth proxy reception.
- Successful publication of battery and charging entities.
- Reproducible custom Docker image with compiled ARM64 Cython support.
- Successful validation following container recreation.

</details>

**Status:** Both proposals are open and submitted for review as of November 26, 2026. The habluetooth proposal currently requires merge-conflict resolution. The Apple BLE proposal depends on acceptance and availability of the upstream API.

**Validation scope:** Hardware testing used a locally patched Bluetooth manager and integration. Official upstream availability, broader scanner compatibility and complete Home Assistant lifecycle validation remain outstanding.

**Impact:** Establishes a proposed integration path for native Apple BLE reception without globally relaxing existing advertisement filtering.

[**habluetooth API proposal #662**](https://github.com/Bluetooth-Devices/habluetooth/pull/662) · [**Apple BLE integration proposal #6**](https://github.com/hudsonbrendon/ha-apple-ble/pull/6)

### Inkcut — Network Serial Transport & Plotter Integration

**Open Source · Python · asyncio · RFC2217 · HPGL · Linux · Raspberry Pi · Hardware Validation**

Investigated a limitation in Inkcut's serial transport while bringing a legacy Refine EH-1351 vinyl cutter into a Linux-based workflow. Developed a network serial transport prototype and proposed a portable device profile in two independent upstream pull requests.

| Upstream contribution | Validation |
| --- | --- |
| [**PR #450 — RFC2217 network serial transport**](https://github.com/inkcut/inkcut/pull/450) | Six new regression tests; 92 tests passed; successful physical SVG pen plot over the network |
| [**PR #451 — Refine EH-1351 device profile**](https://github.com/inkcut/inkcut/pull/451) | Profile and serial defaults validated; all 86 upstream tests passed independently |

<details>
<summary><strong>Explore Inkcut architecture, testing & limitations</strong></summary>

- **Root cause analysis:** Reproduced an unsupported write-timeout operation in the existing serial transport when using RFC2217.
- **Transport engineering:** Proposed a dedicated asynchronous network serial transport with ordered writes, error propagation and configurable serial URLs.
- **Hardware integration:** Connected a CH340 USB serial interface to a Raspberry Pi running ser2net, with Inkcut running on a second Raspberry Pi 5.
- **Remote operation:** Used noVNC through an SSH tunnel for browser-based access to Inkcut.
- **Physical validation:** Plotted a 20 × 20 mm square, 14 mm circle and 6 mm crosshair using HPGL and a pen. Ruler measurements showed approximate dimensional agreement.
- **Independent contributions:** Kept the device profile separate from the transport changes and excluded installation-specific network addresses.

**Validation scope:** Tested on Debian 13 / ARM64 with one Refine EH-1351. Timeout, cancellation and connection-loss handling require further hardening. Direct USB operation with the new native profile, maximum cutting width, blade cutting and repeated passes remain unverified. RFC2217 requires a trusted network or appropriately secured tunnel.

</details>

**Status:** Both upstream PRs were opened for review on November 25, 2026; acceptance was pending at publication.

**Expected impact:** Makes legacy serial hardware more accessible in local Linux workflows and lays a foundation for network-connected plotting across compatible devices.

[**Network transport PR →**](https://github.com/inkcut/inkcut/pull/450) · [Device profile PR](https://github.com/inkcut/inkcut/pull/451)

### SunFounder — Upstream Contributions

**Open Source · Raspberry Pi · Linux · Hardware Integration · Home Assistant · IR / LIRC · Maintainer Collaboration**

Contributing hardware-focused improvements to SunFounder's ecosystem, connecting Linux-level functionality with reproducible smart-home integrations.

**🏆 Key milestone: Listed in SunFounder's official documentation**

On November 24, 2026, SunFounder merged [PR #27](https://github.com/sunfounder/home-assistant-addon/pull/27), introducing a dedicated **Community add-ons** section in its official Home Assistant add-on repository and listing my community-maintained Pironman 5 Max IR receiver add-on.

The listing followed technical collaboration, independent community testing and improvements to the installation experience based on manufacturer feedback.

**From community feedback to manufacturer documentation**

| Stage | Outcome |
| --- | --- |
| **Community need** | Identified demand for Pironman 5 Max infrared receiver support on Home Assistant OS. |
| **Engineering** | Developed a standalone HAOS add-on and companion integration with automated validation and documentation. |
| **Hardware validation** | Received independent community testing with HAOS and HAIR. |
| **Maintainer feedback** | Identified maintenance concerns and unnecessary manual installation steps. |
| **Installation optimization** | Introduced v0.2.0 with direct event-based communication to the existing HACS integration. |
| **Official documentation listing** | SunFounder merged PR #27, making the community-maintained solution discoverable through its official repository. |

<details>
<summary><strong>Explore SunFounder PRs, technical implementation & maintainer collaboration</strong></summary>

**Selected upstream and community contributions**

- [**Pironman 5 Max IR Receiver — upstream PR #26 (closed, not merged)**](https://github.com/sunfounder/home-assistant-addon/pull/26) — Proposed a standalone HAOS infrared receiver add-on and companion integration; independently tested with Home Assistant OS and HAIR.
- [**Official community add-on listing — PR #27 (merged)**](https://github.com/sunfounder/home-assistant-addon/pull/27) — Manufacturer-authored documentation update introducing a Community add-ons section and listing my community-maintained IR receiver add-on, including the simplified installation approach.
- [**OLED / SSD1306 Font Asset Fix**](https://github.com/sunfounder/pm_auto/pull/19) — Corrected an asset path issue in the upstream driver.
- [**Debian Trixie Compatibility**](https://github.com/sunfounder/pironman5/pull/109) — Contributed tested platform compatibility information.

**Technical architecture**

The local infrared receiving pipeline connects the Pironman 5 Max's built-in IR receiver to Home Assistant through GPIO13, LIRC and the appropriate integration layer.

Two deployment approaches address different Home Assistant environments:

| Environment | Implementation |
| --- | --- |
| Home Assistant Container | Linux/LIRC host bridge and native HACS integration |
| Home Assistant OS | Community-maintained IR add-on with direct event-based communication to the existing HACS integration |

Both approaches aim to make the hardware's infrared receiving functionality accessible to Home Assistant users without unnecessary cloud dependencies.

**Installation experience improvements — v0.2.0**

- Introduced the `pironman5` event mode for direct communication with the existing HACS integration.
- Removed the need to manually copy `sunfounder_ir` into `/config/custom_components/`.
- Reduced installation complexity for HAOS users.
- Reused existing integration functionality instead of requiring a separate custom component.
- Updated documentation to reflect the recommended HACS-based installation path.
- Preserved independent maintenance ownership of the community add-on.

</details>

**Maintainer collaboration:** SunFounder positively acknowledged the documentation, automated tests, independent HAOS validation and simplified installation architecture.

Following maintainer feedback, I introduced an event-based integration with the existing HACS component, addressing the concern about manual companion-integration installation.

SunFounder subsequently merged PR #27, officially listing the community-maintained IR add-on in its documentation while keeping maintenance ownership independent.

**Scope:** The IR receiver add-on remains community-maintained and is not an official SunFounder-maintained add-on. The upstream proposal in PR #26 was not merged due to maintenance considerations.

**Impact:** Translating device-specific hardware capabilities into locally usable and documented integrations, reducing installation friction, and establishing a constructive collaboration between independent open-source development and the hardware manufacturer.

[**Official SunFounder community listing →**](https://github.com/sunfounder/home-assistant-addon#community-add-ons) · [Merged documentation PR #27](https://github.com/sunfounder/home-assistant-addon/pull/27) · [Original IR proposal #26](https://github.com/sunfounder/home-assistant-addon/pull/26) · [Native IR / HAIR integration](https://github.com/ChristophKomenda/pironman5-homeassistant-container/blob/main/docs/native-ir-hair.md)

### Powerline2MQTT — Local Powerline Network Monitoring

**Open Source · Python · MQTT · Home Assistant · Docker · Linux · HomePlug AV/AV2 · Raspberry Pi**

Designed and developed a standalone, read-only MQTT bridge that makes compatible Powerline adapters observable without cloud services or adapter IP addresses. The collector runs independently of Home Assistant, using local Ethernet management queries via open-plc-utils.

**Key milestone: v0.1.0-rc.2 — hardware-validated MQTT monitoring**

| Validation | Outcome |
| --- | --- |
| Hardware | Three adapters detected on Raspberry Pi 5 / Debian 13 (TP-Link QCA7420 and two Gongjin-OUI remote stations) |
| Home Assistant | Four devices, **31/31 entities available**, including three connectivity sensors |
| Automated testing | **19 unit tests passed** |
| Reliability | Observed automatic recovery from transient scan failures in approximately five seconds |
| Deployment | ARM64 runtime validated; ARM64 and AMD64 container builds; experimental HAOS packaging |

<details>
<summary><strong>Explore Powerline2MQTT architecture, reliability & developer experience</strong></summary>

- **MQTT-first architecture:** Decouples Layer 2 hardware discovery from Home Assistant, allowing other MQTT clients and remote collectors to consume the data.
- **Automatic discovery:** Adapter topology, TX/RX link rates, network roles, firmware and chipset information where available.
- **Resilient monitoring:** Monotonic polling scheduler, five-second retries, debounced adapter presence and discovery refresh after MQTT reconnect or Home Assistant birth messages.
- **Operational diagnostics:** Session success and failure counters, consecutive failures, polling intervals and last successful scan.
- **Security-conscious deployment:** Read-only management queries, minimal Docker capabilities and no cloud dependencies.
- **Developer experience:** Multi-architecture CI, versioned prereleases, installation and rollback guidance, compatibility documentation and explicit release gates.

</details>

**Validation scope:** RC.2 was tested on one ARM64 installation. Long-term stability, controlled outage tests, AMD64 runtime and HAOS runtime validation remain outstanding. G.hn is not supported; public container image redistribution remains gated pending dependency license review.

**Impact:** Turns otherwise difficult-to-access Powerline link data into actionable smart-home diagnostics, while keeping the collector independent of any single automation platform.

[**Explore Powerline2MQTT →**](https://github.com/ChristophKomenda/powerline2mqtt) · [Releases](https://github.com/ChristophKomenda/powerline2mqtt/releases) · [Release validation](https://github.com/ChristophKomenda/powerline2mqtt/blob/main/docs/RELEASE.md)

### Home Assistant Community Apps — Automated App Distribution

**Open Source · Home Assistant OS · Python · GitHub Actions · CI/CD · Docker · Release Engineering · Developer Experience**

Designed and implemented an independent, source-based Home Assistant OS app catalog that gives users one repository to discover and install multiple local-first applications, while preserving separate upstream projects and release lifecycles.

| App | Purpose | Build targets |
| --- | --- | --- |
| [Powerline2MQTT](https://github.com/ChristophKomenda/powerline2mqtt) | Local Powerline network monitoring | ARM64 / AMD64 |
| [Pironman IR Receiver](https://github.com/ChristophKomenda/home-assistant-addon) | Local infrared reception for Pironman 5 Max | ARM64 |
| [Bitcoin Node Monitor](https://github.com/ChristophKomenda/bitcoin-node-monitor) | Restricted Bitcoin Core RPC monitoring via MQTT | ARM64 / AMD64 |

**Engineering milestone:** Three app packages integrated, eight release-selection tests passed and all six distribution CI checks passed for the third-app integration ([PR #3](https://github.com/ChristophKomenda/home-assistant-apps/pull/3)).

<details>
<summary><strong>Explore distribution architecture, automation & installation UX</strong></summary>

- **Automated release discovery:** Scheduled and manually triggered upstream release checks, with app-specific prerelease policies and downgrade protection.
- **Reviewable updates:** Import published sources from resolved Git commits and create update pull requests instead of merging automatically.
- **Integrity and traceability:** Exact source versions, commit references and SHA-256 content hashes recorded in a lock file.
- **Build validation:** Five native ARM64/AMD64 Docker build targets and separate static package validation.
- **Developer experience:** Shared installation entry point, accessible project documentation, catalog branding, contribution guidelines and security policy.
- **Independent maintenance:** App-specific fixes remain upstream; the central repository owns distribution and catalog presentation.

</details>

**Validation scope:** Static checks and native image builds passed. A no-update synchronization run was successful; importing a newer release and creating a real automatic update PR still need end-to-end confirmation. Central HAOS runtime testing remains pending. Content hashes are integrity checks, not independent signatures or a security audit.

**Impact:** Reduces installation and release-maintenance friction through a reusable distribution architecture, combining product UX with software engineering and transparent release management.

[**Explore Community Apps →**](https://github.com/ChristophKomenda/home-assistant-apps) · [CI workflows](https://github.com/ChristophKomenda/home-assistant-apps/actions) · [Pinned upstream sources](https://github.com/ChristophKomenda/home-assistant-apps/blob/main/SOURCES.md)

### Bitcoin Node Monitor — Local Bitcoin Core Monitoring

**Open Source · Python · Bitcoin Core JSON-RPC · MQTT · TLS · Home Assistant OS · Docker**

Developed an independent monitoring app for existing Bitcoin Core nodes, extending the monitoring concept from Bitcoin Pi Node to a network-based deployment without access to the Docker socket or a privileged container.

<details>
<summary><strong>Explore monitoring features, security & validation</strong></summary>

- **19 MQTT Discovery entities:** Block and header heights, verification progress, peer connections, blockchain data size, uptime, network traffic and sync health indicators.
- **Restricted client-side RPC:** Four monitoring methods only; dedicated server-side method restrictions are also required.
- **Transport security:** TLS support and certificate verification, with insecure connections requiring explicit opt-in.
- **Availability:** MQTT availability, last will and reconnection logic.
- **Deployment:** Experimental HAOS packaging, ARM64/AMD64 build targets and automated distribution through the Community Apps repository.

</details>

**Validation:** Six unit tests passed locally and source-repository CI passed for [v0.1.0-alpha.1](https://github.com/ChristophKomenda/bitcoin-node-monitor/releases/tag/v0.1.0-alpha.1). Live RPC, reconnect behavior and HAOS runtime testing remain outstanding. Remote filesystem free space is deliberately not reported. Bitcoin RPC must not be exposed publicly.

[**Explore Bitcoin Node Monitor →**](https://github.com/ChristophKomenda/bitcoin-node-monitor) · [Experimental release](https://github.com/ChristophKomenda/bitcoin-node-monitor/releases/tag/v0.1.0-alpha.1) · [Community app catalog](https://github.com/ChristophKomenda/home-assistant-apps)

### Bitcoin Pi Node — Secure Self-Hosted Bitcoin Core

**Open Source · Raspberry Pi 5 · Linux · Docker Compose · Bash · systemd · GitHub Actions**

Built a lightweight deployment for a **pruned, validating Bitcoin Core node** on Raspberry Pi 5, with dedicated microSD, SSD or NVMe storage, safer startup controls and optional Home Assistant monitoring.

<details>
<summary><strong>Explore Bitcoin Pi Node security, MQTT, bandwidth & operations</strong></summary>

**Key engineering contributions**

- **Safer startup:** Optional systemd service verifies the mounted filesystem UUID before starting the container, reducing the risk of writing blockchain data to the system drive.
- **Lean architecture:** Configurable pruning, persistent storage and Bitcoin P2P networking without exposing the RPC port on the host.
- **Home Assistant monitoring:** Optional, read-only MQTT Discovery with **21 entities** for sync progress, peers, storage, uptime, traffic and health indicators; scheduled updates via systemd timer.
- **Bandwidth management:** Optional upload/download limiting for the Bitcoin container, without shaping unrelated host services.
- **Operational visibility:** CLI helpers for synchronization status, block height and peer connections.
- **Maintainability:** Storage preflight checks, setup documentation and GitHub Actions covering Bash syntax, ShellCheck and Docker Compose validation.

</details>

**Validation:** Built and tested on Raspberry Pi 5 with Debian 13 and Bitcoin Core 31.1. The MQTT feature and documentation were merged in [PR #5](https://github.com/ChristophKomenda/bitcoin-pi-node/pull/5) and [PR #6](https://github.com/ChristophKomenda/bitcoin-pi-node/pull/6). Full initial synchronization and controlled restart testing are not yet documented as complete.

**Impact:** Making self-hosted Bitcoin infrastructure more approachable through reproducible deployment, safer storage handling and clear operational documentation.

[**Explore Bitcoin Pi Node →**](https://github.com/ChristophKomenda/bitcoin-pi-node) · [Home Assistant setup](https://github.com/ChristophKomenda/bitcoin-pi-node/blob/main/docs/home-assistant.md) · [MQTT monitoring PR](https://github.com/ChristophKomenda/bitcoin-pi-node/pull/5)

---

## How I Work

*From user needs to implementation, testing and measurable improvements.*

**Understand the user → design the experience → build the solution → measure and improve.**

I combine qualitative UX thinking with implementation and analytics. Depending on the project, that means improving task flows and interface clarity, writing HTML/CSS/JavaScript, working with WordPress and WooCommerce, auditing Core Web Vitals, or using GA4 events to understand how people interact with a site.

My open-source contributions follow a similar process: **investigate the problem, validate assumptions, implement a solution, test it and document the results.**

I apply the same user-centered approach to technical products and developer experiences — reducing installation friction, improving documentation, incorporating maintainer feedback and making complex systems easier to understand and operate.

**My focus:** Meaningful outcomes, maintainable implementation and measurable impact. I prefer documented before-and-after evidence over unsupported performance or conversion claims. I also distinguish **tested**, **experimental** and **proposed** functionality when publishing open-source work.

## Skills & Technologies

| Area | Tools and capabilities |
| --- | --- |
| **UX/UI & Product Design** | Figma, Adobe Creative Cloud, responsive design, user journeys, information architecture, prototyping |
| **Frontend** | HTML, CSS, JavaScript, React, accessible and responsive interfaces |
| **E-Commerce & CMS** | WordPress, Elementor, WooCommerce, Shopify, Salesforce Commerce Cloud |
| **SEO & Optimization** | Technical SEO, Schema.org, Core Web Vitals, PageSpeed, conversion rate optimization (CRO) |
| **Analytics** | Google Analytics 4, Google Tag Manager, event tracking and performance analysis |
| **Software Development & Testing** | Python, TypeScript, Node.js, Cython, asyncio, API integration, protocol analysis, automated regression testing, Git, GitHub |
| **Infrastructure & Open Source** | Linux, Docker, Raspberry Pi, Home Assistant, MQTT, TLS / PKI, Mosquitto, Ethernet / HomePlug, RFC2217, HPGL, REST APIs, Nginx, Cloudflare |
| **Bluetooth & Hardware Integration** | Bluetooth LE, BlueZ, D-Bus, HCI controller identity, Bluetooth proxies, advertisement filtering, PipeWire |
| **Observability & Performance Engineering** | Communication diagnostics, MQTT lifecycle management, memory and latency benchmarking, bounded caching, regression coverage, hardware validation |
| **CI/CD & Release Engineering** | GitHub Actions, native multi-architecture Docker builds, versioned upstream imports, SHA-256 integrity checks, reviewable release automation |
| **Developer Experience & Collaboration** | Technical documentation, installation UX, upstream contributions, maintainer feedback, community-driven development |

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

I'm open to **UX/UI, frontend engineering, e-commerce and digital product opportunities**, **selected freelance collaborations**, and **open-source contributions** — especially work connecting user needs, technical implementation and business outcomes.

If you're building a product, improving a digital customer journey or working on a project where design and engineering meet, I'd be happy to connect.

| Interested in | Next step |
| --- | --- |
| Freelance UX, web design or e-commerce projects | [Explore my portfolio and get in touch](https://christophkomenda.de) |
| Hiring or product-team collaboration | [View my CV](https://christophkomenda.de/wp-content/uploads/2026/10/CV_Christoph_Komenda.pdf) |
| Open-source collaboration | [Explore repositories](https://github.com/ChristophKomenda?tab=repositories) |
| Pironman integration and hardware testing | [Join the community discussion](https://github.com/ChristophKomenda/pironman5-homeassistant-container/discussions) |

*Design thoughtfully. Build practically. Improve continuously.*
