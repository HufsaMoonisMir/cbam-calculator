# EUDR Due Diligence Checklist
## EU Deforestation Regulation (EU) 2023/1115 — Operator Compliance Checklist

> **Published by**: [Sustainability-Frisk](https://sustainability-frisk.com) | MIT Licence | Free to use and adapt  
> **Regulation**: Regulation (EU) 2023/1115 of the European Parliament  
> **Enforcement**: Active (large operators) | Delayed for SMEs — confirm current dates at [ec.europa.eu/environment/forests/eudr](https://environment.ec.europa.eu/topics/forests/deforestation/regulation-deforestation-free-products_en)  
> **Last updated**: May 2026

---

## Which Commodities Are Covered?

| Commodity | Products Included | CN Codes (examples) |
|---|---|---|
| **Cattle / Beef** | Live cattle, beef, leather, gelatin, tallow | 0102, 0201, 4104, 4105 |
| **Cocoa** | Cocoa beans, paste, butter, powder, chocolate | 1801, 1802, 1803, 1804, 1806 |
| **Coffee** | All coffee (roasted, green, instant) | 0901 |
| **Palm oil** | Crude/refined palm oil, palm kernel, fractions | 1511, 1513 |
| **Soya** | Soybeans, soya flour, soya oil, soya cake | 1201, 1208, 1507 |
| **Wood** | Timber, paper, pulp, furniture, charcoal | 4401–4421, 4701–4710, 9401, 9403 |
| **Rubber** | Natural rubber (latex), rubber products | 4001, 4002, 4011–4017 |
| **Leather** | Hides from cattle only | 4101–4107 |

> ⚠️ Only **natural rubber** and **leather from cattle** are covered — synthetic rubber and leather from other animals are excluded.

---

## SECTION 1: Information Requirements Checklist

Before submitting a Due Diligence Statement (DDS), confirm you have collected ALL of the following:

### 1.1 Product Information
- [ ] Product description (using Combined Nomenclature CN 8-digit code)
- [ ] Quantity (net weight in kg or volume in litres, as applicable)
- [ ] Country of production (where the commodity was grown/raised)
- [ ] Geolocation data (see Section 2)
- [ ] Supplier name(s) and address(es)
- [ ] Description of operator's due diligence procedures

### 1.2 Geolocation Data — The Core Requirement
This is where most operators fail. EUDR requires:

| Plot Size | Geolocation Required | Format |
|---|---|---|
| < 4 hectares | **One centroid point** (single lat/long coordinate) | WGS84 decimal degrees |
| ≥ 4 hectares | **Polygon** (at minimum 4 vertices tracing the plot boundary) | KML / GeoJSON / WKT |

**How to collect:**
- GPS field visit: use a smartphone GPS app (e.g. Field Area Map, GPS Fields Area Measure)
- Satellite: use Google Earth Pro to draw polygons → export as KML
- Supplier-provided: require your suppliers to submit GPS data as part of purchase order conditions

**Minimum data per plot:**
```
Plot ID: [unique identifier]
Latitude: [decimal degrees, e.g. 3.5678]
Longitude: [decimal degrees, e.g. 101.2345]
Area (ha): [hectares]
Country: [ISO 3166-1 alpha-2 code]
Commodity: [EUDR commodity name]
Production date range: [YYYY-MM-DD to YYYY-MM-DD]
```

### 1.3 Deforestation-Free Verification
- [ ] Production area is NOT in land that was deforested after **31 December 2020**
- [ ] Satellite imagery review completed (see tools below)
- [ ] Country/region risk classification confirmed (see Section 3)

**Free satellite verification tools:**
- [Global Forest Watch](https://www.globalforestwatch.org) — tree cover loss alerts since 2000
- [EU JRC Global Forest Cover](https://forest.jrc.ec.europa.eu) — official EU reference dataset
- [Hansen/UMD Forest Cover 2020](https://earthenginepartners.appspot.com/science-2013-global-forest) — deforestation baseline

---

## SECTION 2: Country Risk Classification

| Risk Level | Countries / Regions | Due Diligence Required |
|---|---|---|
| **Standard risk** | Most producing countries | Full geolocation + risk assessment |
| **Low risk** | Countries with negligible deforestation | Simplified due diligence |
| **High risk** | Countries where deforestation is significant | Enhanced due diligence |

> The EU Commission publishes the official country risk benchmarking. Check the current list at [ec.europa.eu/environment/forests/eudr_benchmarking](https://environment.ec.europa.eu).

### Standard Risk Assessment Questions
Answer YES or NO to each:

**Environmental:**
- [ ] Is the production area free from protected/conservation status? (YES required)
- [ ] Is the land legally registered for agricultural/forestry use? (YES required)
- [ ] Is there no overlap with indigenous/community-protected land? (YES required)
- [ ] Is the production post-2020 land use consistent with satellite data? (YES required)

**Legal:**
- [ ] Does the operator hold legal land tenure or long-term lease? (YES required)
- [ ] Are all required environmental permits held? (YES required)
- [ ] Is third-party/forest area free from disputed ownership? (YES required)

---

## SECTION 3: Risk Mitigation Measures

If any risk question in Section 2 is NO or UNCERTAIN, document the following:

| Risk Identified | Mitigation Action | Evidence Collected | Date Completed |
|---|---|---|---|
| | | | |
| | | | |

**Standard mitigation options:**
- Require supplier audit (RSPO, FSC, Rainforest Alliance, SEDEX)
- Commission independent third-party site visit
- Request satellite imagery covering the deforestation baseline date
- Require supplier declaration with legal tenure evidence

---

## SECTION 4: Due Diligence Statement (DDS) Filing

### What is a DDS?
A Due Diligence Statement is filed per shipment (or per batch of same-commodity shipments in the same reporting period) in the **EU TRACES NT system** before the goods enter the EU.

### DDS Filing Checklist
- [ ] TRACES NT account created (at [food.ec.europa.eu](https://food.ec.europa.eu/plants/eu-trade-system-traces_en))
- [ ] Reference number from supplier's DDS (if importing from another EU operator)
- [ ] All geolocation data uploaded (KML/GeoJSON files attached or coordinates entered)
- [ ] Risk assessment documented and attached
- [ ] Quantity and product description matches shipping documents
- [ ] DDS submitted **before** goods arrive at EU border
- [ ] DDS reference number recorded for 5-year retention

### Document Retention Requirements
Under Article 10 of EUDR, operators must retain all due diligence records for **5 years** from the date of the DDS submission:
- Geolocation data files
- Risk assessment documentation
- Supplier declarations and contracts
- Satellite imagery or verification reports
- TRACES NT submission confirmations

---

## SECTION 5: Supplier Due Diligence Integration

### Supplier Contract Clauses (template language)
Add to purchase orders and supplier contracts:

```
EUDR Compliance Clause

The Supplier warrants that all [commodity] supplied under this agreement:
(a) was produced on land free from deforestation after 31 December 2020;
(b) was produced in compliance with applicable laws of the country of origin 
    including environmental and land-rights legislation;
(c) is accompanied by geolocation data (GPS coordinates or polygon data) 
    identifying the exact plot(s) of production, provided in WGS84 decimal 
    degrees format, within [30] days of purchase order confirmation.

The Supplier agrees to cooperate with any due diligence audit requested by 
[Company Name] or its representatives, and to provide documentary evidence 
of the above warranties within [10] business days of any request.

Failure to provide required geolocation data or to satisfy due diligence 
requirements constitutes a material breach of this agreement.
```

### Supplier Data Request Template
Send to all tier-1 suppliers:

**Subject**: EUDR Geolocation Data Request — [Your company] compliance requirement

*Dear [Supplier name],*

*EU Regulation 2023/1115 (EUDR) requires us to collect the following information for all [commodity] purchases. Please provide this data for all plots supplying our orders:*

| Field | Required | Format |
|---|---|---|
| Farm/plot name or ID | Yes | Text |
| Country | Yes | ISO code |
| Latitude | Yes | Decimal degrees (e.g. 3.5678) |
| Longitude | Yes | Decimal degrees (e.g. 101.2345) |
| Plot area | Yes | Hectares |
| Polygon boundary file | If plot ≥ 4ha | KML or GeoJSON attachment |
| Land title / tenure document | Yes | PDF scan |
| Production year | Yes | YYYY |

---

## Useful References

- [Official EUDR text (EUR-Lex)](https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX%3A32023R1115)
- [EU Commission EUDR guidance page](https://environment.ec.europa.eu/topics/forests/deforestation/regulation-deforestation-free-products_en)
- [TRACES NT system](https://food.ec.europa.eu/plants/eu-trade-system-traces_en)
- [Global Forest Watch](https://www.globalforestwatch.org)
- [Sustainability-Frisk EUDR service (€6,000)](https://sustainability-frisk.com)

---

## About This Checklist

This checklist is published by **Sustainability-Frisk** as a free resource for operators navigating EUDR compliance. It reflects the regulation as enacted and Commission guidance published to May 2026. Regulatory requirements evolve — always verify against the current Commission guidance and Official Journal of the EU.

For a verified, audit-ready EUDR Due Diligence Statement Pack for your specific shipment, see our [EUDR DDS Pack (€249)](https://sustainability-frisk.com/#report-eudr).

**MIT Licence** — free to use, adapt, and redistribute with attribution.
