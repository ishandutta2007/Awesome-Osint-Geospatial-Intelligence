# Awesome-Osint-Geospatial-Intelligence
# Awesome-Osint-Geospatial-Intelligence

# Awesome OSINT & Geospatial Intelligence

> A curated list of top OSINT and Geospatial Intelligence platforms — both SaaS/Hosted commercial solutions and open-source alternatives for geolocation, satellite analysis, maritime tracking, and multi-source intelligence fusion.
> 🌟 Star this repo if you find it useful! 🌟

---

## 📋 Table of Contents

- [SaaS / Hosted Platforms](#-saas--hosted-platforms)
  - [Recorded Future](#recorded-future)
  - [Dataminr](#dataminr)
  - [Janes](#janes)
  - [Maxar Technologies](#maxar-technologies)
  - [Planet Insights](#planet-insights)
  - [BlackSky](#blacksky)
  - [Descartes Labs](#descartes-labs)
  - [Spire Global](#spire-global)
  - [Orbital Insight](#orbital-insight)
  - [HawkEye 360](#hawkeye-360)
- [Open-Source Software](#-open-source-software)
  - [Azimut](#azimut)
  - [TerraScout AI](#terrascout-ai)
  - [Osiris](#osiris)
  - [Neptune AIS](#neptune-ais)
  - [OpenOSINT](#openosint)
  - [Unbihexium](#unbihexium)
  - [SIPT](#sipt)

---

## 🟦 SaaS / Hosted Platforms

Commercial, cloud-hosted OSINT and Geospatial Intelligence platforms. These are not open-source but are included as reference points for feature comparison.

### Recorded Future
**Type:** Real-time threat intelligence with geospatial context
Recorded Future provides intelligence across open, technical, deep, and dark web sources, with geospatial context for threat actors and campaigns. It is positioned for security teams wanting intelligence-driven prioritization with location awareness.

### Dataminr
**Type:** Real-time event detection from public data
Dataminr detects breaking events from public data sources (social media, news, sensors) with geolocation and impact assessment. It is positioned for organizations needing early warning on incidents affecting operations or personnel.

### Janes
**Type:** Defense and security intelligence
Janes provides open-source defense and security intelligence, including order of battle data, equipment profiles, and geospatial analysis. It is positioned for government and defense organizations needing structured, verified intelligence.

### Maxar Technologies
**Type:** High-resolution satellite imagery and analytics
Maxar provides high-resolution satellite imagery, 3D geospatial data, and analytics for defense, intelligence, and commercial applications. It is the long-standing commercial standard for satellite imagery.

### Planet Insights
**Type:** Daily satellite imagery and analytics
Planet operates a large fleet of satellites providing daily imagery of the Earth, with analytics for change detection, agriculture, and environmental monitoring. It is positioned for organizations needing frequent revisit rates.

### BlackSky
**Type:** Real-time satellite imagery and analytics
BlackSky provides high-revisit satellite imagery with AI-powered analytics for defense, intelligence, and critical infrastructure monitoring. It is positioned for time-sensitive geospatial intelligence.

### Descartes Labs
**Type:** Geospatial analytics platform
Descartes Labs provides a cloud platform for analyzing satellite imagery at scale, with tools for environmental monitoring, agriculture, and supply chain analysis. It is positioned for data scientists working with geospatial data.

### Spire Global
**Type:** Satellite-powered maritime and weather data
Spire operates a constellation of nanosatellites providing maritime AIS data, weather data, and aviation tracking. It is positioned for organizations needing global maritime domain awareness.

### Orbital Insight
**Type:** Geospatial analytics with AI
Orbital Insight analyzes satellite imagery and geolocation data to provide insights on economic activity, infrastructure, and supply chains. It is positioned for organizations wanting macro-level geospatial intelligence.

### HawkEye 360
**Type:** Radio frequency geolocation intelligence
HawkEye 360 operates a satellite constellation that geolocates radio frequency signals (maritime radar, VHF, etc.) for maritime domain awareness and defense intelligence. It is positioned for organizations needing RF-based geospatial intelligence.

---

## 🟩 Open-Source Software

Self-hosted, community-driven OSINT and Geospatial Intelligence tools. The open-source ecosystem spans **geolocation workspaces**, **multi-source intelligence dashboards**, **maritime tracking platforms**, **AI-powered reconnaissance frameworks**, and **satellite image processing libraries**.

### Azimut
**Stack:** Python / Svelte / SQLite | **License:** Open Source (PyPI)
Azimut is a local-first **GeoOSINT workspace** for geolocation investigations, keeping all evidence together in a single case folder on your machine . Key capabilities include:
- **Horizon matching**: Stand at any point on the map and see the 3D terrain and skyline visible from that spot up to ~150 km, then overlay the photo being investigated to match peaks and horizon by eye or with the Fit tool 
- **Find (Beta)**: Draw the skyline on a photo, mark an area up to **10,000 km²**, and Azimut ranks places where the hills and ridges best match that skyline 
- **Sun and moon conditions**: Calculate local sun and moon conditions offline and review their daily paths on the map 
- **Proof composition**: Export selected notes as server-rendered PDFs with local images and diagrams, and compose proofs as collages with satellite view and photo 
- **Case management**: Each investigation has its own case, with media placed in that case to prevent confusion 
- **Cross-platform**: Runs on Linux, Windows, and macOS, with self-contained binaries available (no Python required) 

**Trade-off:** Find is still in Beta and limited to 10,000 km² areas; results require human verification .  
**Best for:** OSINT analysts and geolocation investigators wanting a local, evidence-centric workspace with horizon matching and proof composition capabilities.

### TerraScout AI
**Stack:** Python / Streamlit / SAM2 | **License:** Open Source (GitHub)
TerraScout AI is an open-source **geospatial intelligence platform** with **313+ modules**, AI satellite analysis, and real-time monitoring . Key capabilities include:
- **AI satellite image analysis**: Powered by Segment Anything Model (SAM/SAM2), detect and segment objects using text prompts (e.g., "tree", "building", "solar panel"), with batch processing and GeoJSON/CSV/PNG export 
- **Remote structure explorer**: Multi-source search across OpenStreetMap, Google Open Buildings (1.8B AI-detected buildings), Microsoft Building Footprints (1B+ ML-detected buildings), and AI live detection 
- **Satellite imagery viewer**: NASA GIBS (MODIS, VIIRS, NDVI), EOX Sentinel-2 Cloudless (2018-2024 at 10m resolution), tile stitching, and date comparison 
- **Earth monitoring**: Weather, air quality, active wildfires (NASA FIRMS), natural disasters (GDACS), volcanoes, space weather, ISS tracking, near-Earth asteroids 
- **Marine & ocean**: Vessel tracking, tides (NOAA CO-OPS), ocean data 
- **Fusion Console**: 34 analytical sections, 35 algorithms, 40+ data sources in one view 

**Trade-off:** Requires 8 GB RAM minimum (16 GB recommended for AI features), and the project appears to be a single-developer effort with a very recent creation date.  
**Best for:** Analysts wanting a comprehensive, module-rich OSINT dashboard with AI-powered satellite analysis and multi-source data fusion.

### Osiris
**Stack:** Next.js / TypeScript / MapLibre GL / WebGL | **License:** MIT 
Osiris is an open-source **OSINT platform** that aggregates publicly available geospatial information into a single interactive operational dashboard, running locally on a regular laptop without dedicated server infrastructure . Key capabilities include:
- **15+ switchable data layers**: Aircraft and maritime data, satellite wildfire data, infrastructure data, submarine internet cables, seismology, air quality, conflict data, and CCTV 
- **Network reconnaissance tools**: TCP port scanning, DNS records retrieval, WHOIS query, SSL/TLS inspection, service discovery, and vulnerability scanning 
- **GPU-rendered globe**: WebGL-based visualization of ~19,000 objects, with 3D terrain and smooth camera controls 
- **RECON → FINGERPRINT**: Live public-profile search across 462 platforms for username, email, or phone, with soft-404 detection and CSV/JSON export 
- **Live Alerts**: Pinned to named locations with playable footage in place 
- **Local processing**: Most computation on the user's machine, minimizing server costs 

**Trade-off:** The developers note dual-use capabilities—it can be used for legitimate investigations and emergency response, but also for reconnaissance or malicious purposes .  
**Best for:** Investigators and analysts wanting a comprehensive, self-hosted OSINT dashboard with network recon tools and multi-source geospatial layers.

### Neptune AIS
**Stack:** Python / Polars / DuckDB | **License:** Open Source (PyPI)
Neptune AIS is an open-source **maritime intelligence platform** for real-time vessel tracking and AIS data analysis . Key capabilities include:
- **Six open AIS data sources**: NOAA (US waters), Danish Maritime Authority (European waters), Global Fishing Watch (global satellite AIS), Digitraffic Finland, AISHub, and AISStream (real-time WebSocket) 
- **Multi-source fusion**: Combine sources with automatic deduplication ("best", "union", or "prefer" merge strategies) 
- **Event detection**: Port calls, EEZ crossings, encounters, and loitering with confidence scores and full provenance 
- **Real-time streaming**: WebSocket-based ingestion with Parquet sinks and canonical storage promotion 
- **Query interface**: Polars LazyFrame or SQL via DuckDB for large-scale analysis 
- **Plugin system**: Add custom AIS data adapters via Python entry points 

**Trade-off:** Requires API keys for some sources (Global Fishing Watch, AISHub, AISStream), and the platform is focused specifically on maritime AIS data rather than broader geospatial intelligence.  
**Best for:** Maritime analysts and OSINT investigators needing programmatic access to AIS vessel tracking data with multi-source fusion and event detection.

### OpenOSINT
**Stack:** Python / MCP | **License:** Open Source (PyPI)
OpenOSINT is an open-source **OSINT agent** for investigators and security researchers, with **21 public-source tools** behind a natural-language interface and an MCP server . Key capabilities include:
- **Passive by default**: Tools query third-party sources or compute locally; anything that touches the target is off until explicitly opted in (`--allow-active`) 
- **DNS/RDAP/WHOIS lookups**: Records, SPF, DMARC, registrar data, name servers 
- **IP intelligence**: Hostname, ASN, city, geolocation, ISP, proxy/VPN/Tor flags 
- **Geolocated news**: GDELT geolocated news mentions 
- **Breach and reputation**: HaveIBeenPwned, VirusTotal, AbuseIPDB, Shodan, Censys 
- **Web UI with 3D globe**: Agent investigation lands as a point on a globe; entity graph with statement-level provenance 
- **MCP server**: Use from Claude Code, Cursor, or any MCP client 

**Trade-off:** Only passive tools are on by default, and some tools require API keys (Shodan, Censys, VirusTotal, etc.). The tool is focused on entity/network OSINT rather than satellite imagery or terrain analysis.  
**Best for:** Investigators wanting a natural-language OSINT agent with a broad set of passive reconnaissance tools and MCP integration.

### Unbihexium
**Stack:** Python / ONNX / PyTorch | **License:** Open Source (PyPI)
Unbihexium is a Python package for **geospatial machine learning** and satellite image processing, providing input/output, preprocessing, indices, SAR, terrain, geostatistics, analysis, metrics, visualisation, and a model zoo . Key capabilities include:
- **Model zoo**: A catalogue of models for satellite imagery analysis 
- **REST service**: FastAPI-based serving for model inference 
- **Container image**: Available on GitHub Container Registry (`ghcr.io/unbihexium-oss/unbihexium`) 
- **No system GDAL required**: Binary wheels bundle GDAL, PROJ, GEOS, and native libraries 
- **ONNX inference**: Run exported models without PyTorch 

**Important:** The project does not ship trained weights, labelled training data, or imagery, and makes no claim of fitness for operational or safety-critical purposes .  
**Best for:** Developers and researchers building custom geospatial ML pipelines who want a well-structured Python library with model zoo and serving capabilities, accepting that they must supply their own trained weights and data.

### SIPT
**Stack:** Python / RasterIO | **License:** Open Source (Zenodo)
SIPT (Satellite Image Processing Tools) is a Python package that streamlines retrieval and processing of satellite imagery, built on RasterIO without requiring external GDAL installation . Key capabilities include:
- **Mass processing**: Optimized for CPU and GPU multiprocessing of satellite data 
- **Time-series creation**: Simplifies building time-series datasets for environmental monitoring, urban planning, agriculture, and climate analysis 
- **Lightweight setup**: No external GDAL dependency 

**Best for:** Researchers and analysts needing a lightweight Python toolkit for satellite image retrieval and time-series processing, accepting a narrower scope than full OSINT platforms.

---

## 📊 Comparison at a Glance

| Software | License | Stack | Geolocation | Satellite/AI | Maritime | Self-Hosted | Best For |
|----------|---------|-------|-------------|--------------|----------|-------------|----------|
| **Recorded Future** | Proprietary | Cloud | ✅ (Context) | ❌ | ❌ | ❌ | Threat intel + geospatial |
| **Maxar** | Proprietary | Cloud | ✅ | ✅ High-res | ❌ | ❌ | Commercial satellite imagery |
| **Planet** | Proprietary | Cloud | ✅ | ✅ Daily | ❌ | ❌ | Daily revisit imagery |
| **Spire** | Proprietary | Cloud | ✅ | ❌ | ✅ AIS | ❌ | Global maritime AIS |
| **HawkEye 360** | Proprietary | Cloud | ✅ | ❌ | ✅ RF | ❌ | RF geolocation |
| **Azimut** | Open Source | Python/Svelte | ✅ Horizon | ❌ | ❌ | ✅ | Local geolocation workspace |
| **TerraScout AI** | Open Source | Python/SAM2 | ✅ | ✅ AI segmentation | ✅ Vessel tracking | ✅ | 313+ module OSINT dashboard |
| **Osiris** | MIT | Next.js/WebGL | ✅ | ✅ Satellite layers | ✅ Maritime layer | ✅ | GPU globe + network recon |
| **Neptune AIS** | Open Source | Python/Polars | ❌ | ❌ | ✅ Multi-source AIS | ✅ | Programmatic AIS analysis |
| **OpenOSINT** | Open Source | Python/MCP | ✅ (GDELT) | ❌ | ❌ | ✅ | Natural-language OSINT agent |
| **Unbihexium** | Open Source | Python/ONNX | ❌ | ✅ Model zoo | ❌ | ✅ | Geospatial ML library |
| **SIPT** | Open Source | Python/RasterIO | ❌ | ✅ Processing | ❌ | ✅ | Satellite time-series |

---

## 🤝 Contributing

Contributions are welcome! If you know of an open-source OSINT or Geospatial Intelligence tool that should be listed here, please open a pull request with:

- Project name and URL
- Brief description (1–2 sentences)
- Stack and license
- Why it stands out

Please ensure the project is actively maintained (releases within the last 12 months) and genuinely open-source.

**Note on the open-source ecosystem:** The open-source landscape for **OSINT and geospatial intelligence** is **fragmented across distinct capabilities** rather than unified platforms. **Azimut** is the most purpose-built open-source tool for **geolocation investigations**, with horizon matching, skyline finding, and proof composition running entirely locally . **TerraScout AI** and **Osiris** offer the broadest multi-source OSINT dashboards, with TerraScout emphasizing AI satellite segmentation and Osiris emphasizing GPU-rendered globes and network reconnaissance . For **maritime intelligence**, **Neptune AIS** provides programmatic multi-source AIS fusion with event detection . **OpenOSINT** fills the natural-language agent niche with 21 passive reconnaissance tools and MCP integration . **Unbihexium** and **SIPT** serve developers building custom geospatial ML pipelines and satellite processing workflows. No single open-source project fully replicates the commercial satellite constellations of Maxar or Planet, but these tools cover the core geolocation, imagery analysis, and multi-source intelligence workflows for self-hosted deployments.

---

## 📄 License

This list is released under CC0 1.0 Universal (Public Domain). The software projects listed retain their respective licenses.

---

⭐ **If this list helped you discover a useful tool, please star the repo!** ⭐
