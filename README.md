# Christoph Komenda

**UX/UI Designer & Frontend Developer** · Digital Products · E-Commerce · Open Source Engineering

I design and build user-centered digital products that make complex tasks easier — from e-commerce customer journeys to local-first IoT and Home Assistant integrations. I connect user experience, frontend development, technical SEO, conversion optimization and maintainable software engineering.

[**View portfolio**](https://christophkomenda.de) · [**View CV (PDF)**](https://christophkomenda.de/wp-content/uploads/2026/10/CV_Christoph_Komenda.pdf) · [Get in touch](#lets-build-something-useful)

Open to UX/UI, frontend, e-commerce and digital product opportunities, selected freelance projects and open-source collaboration.

## Verified milestones

- **[HACS default repository acceptance](https://github.com/hacs/default/pull/12242)** — independently developed Pironman Home Assistant integration.
- **[SunFounder community listing](https://github.com/sunfounder/home-assistant-addon#community-add-ons)** — community-maintained IR add-on listed in manufacturer documentation; not manufacturer-maintained.
- **[24 read-only Weishaupt sensors merged upstream](https://github.com/kraiz/hassio-weishaupt/pulls?q=is%3Apr+author%3AChristophKomenda)** — three merged protocol and monitoring contributions.

## Start here

- **Hiring & product teams:** [Professional background](#background) · [Skills](#skills--technologies) · [UX and e-commerce projects](#uxui-design-and-e-commerce)
- **Businesses & clients:** [Client projects](#uxui-design-and-e-commerce) · [How I work](#how-i-work) · [Portfolio and contact](https://christophkomenda.de)
- **Developers & maintainers:** [Home Assistant projects](#home-assistant-and-local-first-open-source) · [Upstream contributions](#upstream-contributions-and-hardware-engineering) · [All repositories](https://github.com/ChristophKomenda?tab=repositories)

## Featured projects

- [DNATest.ch](#dnatestch--uxui--e-commerce-relaunch) — e-commerce UX, technical SEO and conversion-oriented design.
- [Pironman 5 / 5 Max](#pironman-5--5-max--home-assistant-integration) — HACS integration and hardware usability.
- [Infrastructure HA Monitor](#infrastructure-ha-monitor--distributed-infrastructure-observability) — distributed observability and operational diagnostics.
- [Weishaupt WTC](#weishaupt-wtc--protocol-reverse-engineering--upstream-contributions) — hardware-validated protocol contributions.

Status labels summarize the evidence recorded in this profile, not a live upstream review. Proposed functionality is not presented as merged or released. Expand project details for validation scope, limitations and source links.


## UX/UI design and e-commerce


### DNATest.ch — UX/UI & E-Commerce Relaunch

**Status:** Client project

Clearer Swiss DNA-testing purchasing journeys through product UX, WooCommerce, SEO and CRO.

[Explore DNATest.ch](https://dnatest.ch)


<details>
<summary>Project details, evidence and validation scope</summary>

**Focus: Making complex product decisions clearer and easier to navigate.**

**UX/UI · WordPress · WooCommerce · HTML · CSS · JavaScript · SEO · CRO**

Redesigned and optimized a Swiss DNA-testing e-commerce experience, focusing on clarity, trust, accessibility of product information and the path from discovery to purchase.

- Reworked content hierarchy, navigation, product presentation and calls to action
- Improved responsive layouts and reusable frontend components
- Implemented structured data and technical SEO enhancements
- Focused on page performance, usability and conversion-oriented journeys

[**Explore DNATest.ch →**](https://dnatest.ch)

</details>


### SR Brennholzhandel — Local Business Website Optimization

**Status:** Client project

Mobile-friendly local commerce, clearer delivery information and contact journeys.

[Explore SR Brennholzhandel](https://sr-brennholz.de)


<details>
<summary>Project details, evidence and validation scope</summary>

**Focus: Helping local customers find products, delivery information and contact options quickly.**

**Web Design · WordPress · Frontend · Local SEO · GA4 · CRO**

Built and optimized a regional firewood supplier's digital presence to make products, delivery details and contact options easier to understand and act on.

- Improved information architecture and mobile user journeys
- Introduced prominent contact options and conversion-focused calls to action
- Implemented structured data and analytics event tracking
- Worked on frontend performance and technical SEO

[**Visit SR Brennholzhandel →**](https://sr-brennholz.de)

</details>


## Home Assistant and local-first open source


### Pironman 5 / 5 Max — Home Assistant Integration

**Status:** HACS accepted · hardware validated; optional IR experimental

Local Raspberry Pi hardware monitoring and control, with HACS discovery and documented compatibility.

[Explore Pironman 5 / 5 Max](https://github.com/ChristophKomenda/pironman5-homeassistant-container)


<details>
<summary>Project details, evidence and validation scope</summary>

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

**Upstream API proposal — persistent host identity**

[SunFounder Pironman #130](https://github.com/sunfounder/pironman5/pull/130) proposes an optional, board-derived `device_uid` for stable third-party integration identity, including a potential Home Assistant Core integration.

The existing product model identifier remains unchanged. This is an open upstream proposal, not an accepted API contract or a Core integration.

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

</details>


### Infrastructure HA Monitor — Distributed Infrastructure Observability

**Status:** Released v1.0.0 · two-host validation

Distributed infrastructure monitoring and incident correlation; 69 passing tests at initial release.

[Explore Infrastructure HA Monitor](https://github.com/ChristophKomenda/infrastructure-ha-monitor)


<details>
<summary>Project details, evidence and validation scope</summary>

**Open Source · Python · MQTT · SQLite · Linux · Raspberry Pi · Docker · Cloudflare · Home Assistant · GitHub Actions**

Designed and developed a distributed monitoring system in response to intermittent website and Cloudflare Tunnel outages, turning real operational problems into actionable infrastructure diagnostics.

**Key milestone: [v1.0.0 — Initial Public Release](https://github.com/ChristophKomenda/infrastructure-ha-monitor/releases/tag/v1.0.0), November 27, 2026**

| Validation | Outcome |
| --- | --- |
| Live deployment | Two Raspberry Pi monitoring agents and one correlation engine |
| Home Assistant | 159 matching entities observed through the API, 154 with known states |
| Automated testing | 69 tests passed on both hosts; GitHub Actions CI passed |
| Persistence | SQLite integrity verified and both hosts registered for persistent boot tracking |

<details>
<summary><strong>Explore distributed architecture, incident correlation & operational diagnostics</strong></summary>

- **Network and application observability:** DNS, ICMP latency and packet loss, HTTP response times, verified public HTTPS certificates, Cloudflare Tunnel redundancy and dynamic TCP edge probes.
- **Cross-host correlation:** Configurable two-host architecture, fresh snapshot validation and rule-based symptom classification.
- **Persistent observability:** SQLite incident history, confirmed recovery tracking, MTTR, MTBF, uptime and measurement coverage.
- **Host and container diagnostics:** Boot-ID changes, observed reboot counters, CPU temperature, Raspberry Pi power flags, filesystem mounts and Docker restart/OOM indicators.
- **Deployment and security:** Native MQTT Discovery, optional certificate-verified MQTT TLS, systemd management scripts and automated CI.

</details>

**Validation scope:** Live deployment on two Raspberry Pi hosts. Full clean-install testing, live MQTT TLS validation and long-term stability testing remain outstanding. Correlation identifies symptoms rather than proving root cause.

**Impact:** Makes intermittent infrastructure failures easier to investigate through a unified, local monitoring workflow in Home Assistant.

[**Explore Infrastructure HA Monitor →**](https://github.com/ChristophKomenda/infrastructure-ha-monitor) · [v1.0.0 release](https://github.com/ChristophKomenda/infrastructure-ha-monitor/releases/tag/v1.0.0) · [CI workflows](https://github.com/ChristophKomenda/infrastructure-ha-monitor/actions)

</details>


### Home Assistant Community Apps — Automated App Distribution

**Status:** Published catalog · HAOS runtime validation pending

Four community-maintained local-first apps with reviewable release automation.

[Explore Home Assistant Community Apps](https://github.com/ChristophKomenda/home-assistant-apps)


**Four apps:** [Powerline2MQTT](https://github.com/ChristophKomenda/powerline2mqtt) · [Pironman IR Receiver](https://github.com/ChristophKomenda/home-assistant-addon) · [Bitcoin Node Monitor](https://github.com/ChristophKomenda/bitcoin-node-monitor) · [Infrastructure HA Monitor](https://github.com/ChristophKomenda/infrastructure-ha-monitor)


<details>
<summary>Project details, evidence and validation scope</summary>

**Open Source · Home Assistant OS · Python · GitHub Actions · CI/CD · Docker · Release Engineering · Developer Experience**

Designed and implemented an independent, source-based Home Assistant OS app catalog that gives users one repository to discover and install multiple local-first applications, while preserving separate upstream projects and release lifecycles.

| App | Purpose | Build targets |
| --- | --- | --- |
| [Powerline2MQTT](https://github.com/ChristophKomenda/powerline2mqtt) | Local Powerline network monitoring | ARM64 / AMD64 |
| [Pironman IR Receiver](https://github.com/ChristophKomenda/home-assistant-addon) | Local infrared reception for Pironman 5 Max | ARM64 |
| [Bitcoin Node Monitor](https://github.com/ChristophKomenda/bitcoin-node-monitor) | Restricted Bitcoin Core RPC monitoring via MQTT | ARM64 / AMD64 |
| [Infrastructure HA Monitor](https://github.com/ChristophKomenda/infrastructure-ha-monitor) | Distributed infrastructure monitoring and cross-host MQTT correlation | See app catalog for current build targets |

**Historical engineering milestone (third-app integration):** Three app packages integrated, eight release-selection tests passed and all six distribution CI checks passed for the third-app integration ([PR #3](https://github.com/ChristophKomenda/home-assistant-apps/pull/3)).

<details>
<summary><strong>Explore distribution architecture, automation & installation UX</strong></summary>

- **Automated release discovery:** Scheduled and manually triggered upstream release checks, with app-specific prerelease policies and downgrade protection.
- **Reviewable updates:** Import published sources from resolved Git commits and create update pull requests instead of merging automatically.
- **Integrity and traceability:** Exact source versions, commit references and SHA-256 content hashes recorded in a lock file.
- **Historical build validation (three-app milestone):** Five native ARM64/AMD64 Docker build targets and separate static package validation.
- **Developer experience:** Shared installation entry point, accessible project documentation, catalog branding, contribution guidelines and security policy.
- **Independent maintenance:** App-specific fixes remain upstream; the central repository owns distribution and catalog presentation.

</details>

**Historical validation scope (three-app milestone):** Static checks and native image builds passed. A no-update synchronization run was successful; importing a newer release and creating a real automatic update PR still need end-to-end confirmation. Central HAOS runtime testing remains pending. Content hashes are integrity checks, not independent signatures or a security audit.

**Impact:** Reduces installation and release-maintenance friction through a reusable distribution architecture, combining product UX with software engineering and transparent release management.

[**Explore Community Apps →**](https://github.com/ChristophKomenda/home-assistant-apps) · [CI workflows](https://github.com/ChristophKomenda/home-assistant-apps/actions) · [Pinned upstream sources](https://github.com/ChristophKomenda/home-assistant-apps/blob/main/SOURCES.md)

</details>


### Powerline2MQTT — Local Powerline Network Monitoring

**Status:** Prerelease · hardware validated on ARM64

Read-only Powerline adapter monitoring through local Ethernet and MQTT discovery.

[Explore Powerline2MQTT](https://github.com/ChristophKomenda/powerline2mqtt)


<details>
<summary>Project details, evidence and validation scope</summary>

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

</details>


### Bitcoin Node Monitor — Local Bitcoin Core Monitoring

**Status:** Experimental alpha · live RPC and HAOS validation pending

Restricted Bitcoin Core RPC monitoring with Home Assistant MQTT discovery.

[Explore Bitcoin Node Monitor](https://github.com/ChristophKomenda/bitcoin-node-monitor)


<details>
<summary>Project details, evidence and validation scope</summary>

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

</details>


### Bitcoin Pi Node — Secure Self-Hosted Bitcoin Core

**Status:** Hardware tested · full synchronization not yet documented

Reproducible pruned Bitcoin Core deployment on Raspberry Pi with guarded storage startup.

[Explore Bitcoin Pi Node](https://github.com/ChristophKomenda/bitcoin-pi-node)


<details>
<summary>Project details, evidence and validation scope</summary>

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

</details>


## Upstream contributions and hardware engineering


### Weishaupt WTC — Protocol Reverse Engineering & Upstream Contributions

**Status:** Merged contributions · additional proposals under review in original evidence

24 read-only sensors merged upstream for heating system monitoring.

[Explore Weishaupt WTC](https://github.com/kraiz/hassio-weishaupt/pulls?q=is%3Apr+author%3AChristophKomenda)


<details>
<summary>Project details, evidence and validation scope</summary>

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
- **Gateway read reliability:** Proposed reducing CanApiJson read batches from six to five parameters in [PR #19](https://github.com/JS-DE-Tech/hacs-weishaupt-lan/pull/19), preserving the existing request gap, register definitions and write behavior.

**WEM-SG hardware validation — November 27, 2026**

| Metric | Before | After |
| --- | ---: | ---: |
| Maximum read batch size | 6 | 5 |
| Available sensors | 50/63 | 57/63 |
| Unavailable or unknown sensors | 13 | 6 |
| Sensor availability | 79.4% | 90.5% |

- Reproduced sixth-slot register rejection on physical WEM-SG hardware.
- Recovered previously unavailable heating and pump readings.
- Validated heating energy against independent energy counters.
- 64 automated tests and 24 subtests passed.
- Added regression coverage for sixth-slot rejection.
- Preserved existing controller write behavior.

**Trade-offs and limitations:** Approximately 20% more HTTP requests for large parameter lists. Hardware validation included a Home Assistant restart. Broader firmware compatibility and isolation of the restart effect remain outstanding.

**Status:** Open upstream compatibility proposal.

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

</details>


### SunFounder — Upstream Contributions

**Status:** Merged documentation listing · API proposal recorded separately

Manufacturer community listing and proposed persistent hardware identity.

[Explore SunFounder](https://github.com/sunfounder/home-assistant-addon#community-add-ons)


<details>
<summary>Project details, evidence and validation scope</summary>

<details>
<summary><strong>Persistent host identity API proposal — November 27, 2026</strong></summary>

[**Pironman PR #130**](https://github.com/sunfounder/pironman5/pull/130) proposes an optional persistent `device_uid` for third-party integrations.

- **Stable identity:** Board-derived identifier independent of network configuration.
- **Privacy-conscious design:** Versioned SHA-256 namespace without exposing the original hardware serial.
- **Backward compatibility:** Existing product identifier and API fields preserved.
- **Automated validation:** 26/26 local tests passed.
- **Product coverage:** All seven upstream product definitions software-tested.
- **Physical validation:** Two Raspberry Pi 5 hosts with Pironman 5 Max enclosures.
- **REST API validation:** 20 repeated HTTP requests, service restart and existing endpoint checks.
- **Package engineering:** Successful wheel build and isolated installation.
- **Operational safety:** Controlled temporary deployment and verified rollback.

**Validation scope:** The UID algorithm was tested across a physical reboot; the patched API was tested across a service restart. Physical HAOS testing, additional hardware variants, actual network reconfiguration and a full reboot of the patched application remain outstanding.

**Identity semantics:** The pseudonymous identifier represents the Raspberry Pi host board, not the enclosure, and is not an authentication credential.

**Status:** Open for maintainer review and agreement on the proposed API contract.

</details>


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

</details>


### hm2mqtt — Battery Communication Diagnostics

**Status:** Proposal · hardware and automated validation recorded

Battery communication diagnostics and recovery observations.

[Explore hm2mqtt](https://github.com/tomquist/hm2mqtt/pull/490)


<details>
<summary>Project details, evidence and validation scope</summary>

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

</details>


### GroBro — Secure MQTT & Solar Infrastructure

**Status:** Proposals · validation recorded

Secure MQTT transport and solar infrastructure deployment improvements.

[Explore GroBro](https://github.com/robertzaage/GroBro/pulls?q=is%3Apr+author%3AChristophKomenda)


<details>
<summary>Project details, evidence and validation scope</summary>

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

</details>


### Tado Hijack — Climate Control & Upstream Contribution

**Status:** Implemented upstream in dev.17, per maintainer

Temperature-step precision improvement.

[Explore Tado Hijack](https://github.com/banter240/tado_hijack/pull/217)


<details>
<summary>Project details, evidence and validation scope</summary>

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

</details>


### Sendspin Bluetooth Bridge — UX & Hardware Performance

**Status:** Proposals · hardware validation recorded

Configuration UX and Bluetooth adapter resolution improvements.

[Explore Sendspin Bluetooth Bridge](https://github.com/trudenboy/sendspin-bt-bridge/pull/605)


<details>
<summary>Project details, evidence and validation scope</summary>

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

</details>


### habluetooth & Apple BLE — Native Bluetooth Reception

**Status:** Coordinated proposals · validation recorded

Optional native Bluetooth reception for compatible Apple BLE devices.

[Explore habluetooth & Apple BLE](https://github.com/Bluetooth-Devices/habluetooth/pull/662)


<details>
<summary>Project details, evidence and validation scope</summary>

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

</details>


### Inkcut — Network Serial Transport & Plotter Integration

**Status:** Proposals · physical plotting validation recorded

Network serial transport and plotter integration.

[Explore Inkcut](https://github.com/inkcut/inkcut/pull/450)


<details>
<summary>Project details, evidence and validation scope</summary>

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

</details>


## Background

My professional background spans **UX/UI design, e-commerce, digital marketing and frontend development**, supported by training in business and IT and continued professional development in UX design, frontend technologies and digital product delivery.

I enjoy working at the intersection of **design, technology and business outcomes** — both in client-facing projects and in open-source communities.

[**See my experience and qualifications →**](https://christophkomenda.de/wp-content/uploads/2026/10/CV_Christoph_Komenda.pdf)


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


## How I Work

*From user needs to implementation, testing and measurable improvements.*

**Understand the user → design the experience → build the solution → measure and improve.**

I combine qualitative UX thinking with implementation and analytics. Depending on the project, that means improving task flows and interface clarity, writing HTML/CSS/JavaScript, working with WordPress and WooCommerce, auditing Core Web Vitals, or using GA4 events to understand how people interact with a site.

My open-source contributions follow a similar process: **investigate the problem, validate assumptions, implement a solution, test it and document the results.**

I apply the same user-centered approach to technical products and developer experiences — reducing installation friction, improving documentation, incorporating maintainer feedback and making complex systems easier to understand and operate.

**My focus:** Meaningful outcomes, maintainable implementation and measurable impact. I prefer documented before-and-after evidence over unsupported performance or conversion claims. I also distinguish **tested**, **experimental** and **proposed** functionality when publishing open-source work.


## More Projects

- [Sabine Hett](https://sabinehett.de) — local SEO, structured data and UX improvements
- [Physio-Aktiv](https://physio-aktiv-ck.de) — digital presence for physiotherapy and health services
- [Business Power Netzwerk](https://businesspowernetzwerk.de) — business website and digital presence
- [Digital CFO](https://www.digital-cfo.eu) — business website and digital presence
- [React frontend capstone](https://github.com/ChristophKomenda/final_project) — component-based React project
- [Christoph Komenda Design](https://christophkomenda.de) — portfolio and independent digital design work


## Additional evidence and history

[Original profile and milestone history (November 27, 2026)](docs/profile-evidence-2026-11-27.md) — preserved source snapshot, including earlier navigation, milestone tables and all original technical claims and links.


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
