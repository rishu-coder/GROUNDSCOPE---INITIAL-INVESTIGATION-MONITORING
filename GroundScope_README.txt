GROUNDSCOPE - INITIAL INVESTIGATION & MONITORING DASHBOARD

Open GroundScope_Dashboard.html in a modern desktop browser. Plotly is bundled; no installation or internet connection is needed for the dashboard. The external research link is optional.

1. Download the blank CSV templates from Data & validation.
2. Populate them with real project records, retaining the exact column names.
3. Upload the relevant CSVs. Datasets can be used independently.
4. Declare your coordinate reference/datum, choose an asset and monitoring cut-off.
5. Review property records, displacement histories, finite-difference rates and spatial geometry.
6. Complete report narrative fields, refresh the draft and download the text report or use browser Print to save PDF.
7. Export filtered records before closing. No automatic session persistence is implemented.

UNITS AND CONVENTIONS
Geometry/reference coordinates: metres in one consistent coordinate reference system.
Displacements: millimetres relative to a declared sensor reference timestamp.
Depths: metres below ground, positive downwards.
Material property units: explicit per record; no automatic conversion.
Timestamps: ISO 8601 with seconds and Z or explicit UTC offset. Cut-off control is UTC.
Monitoring coordinates/reference must remain consistent per sensor. Re-baselined instruments require a separate sensor identifier or externally reconciled data.
Thresholds: optional per observation, resultant magnitude only. Supply amber and red together, with 0 <= amber < red. They must be project-approved outside this application. A value at a threshold counts as an exceedance. Below threshold does not imply safety.
Quality flags are retained and displayed, not automatically accepted or rejected.

CAPABILITIES AND LIMITATIONS
Structured CSV property extraction, filtering and provenance display only. No PDF/OCR or AGS import.
3D viewer: supplied polylines and latest sensor points; not a calibrated predictive digital twin, BIM mesh, geological interpolation or live feed.
No inferred soil strength/stiffness/permeability from displacement, no finite-element solver, no inverse analysis, no slope factor of safety or EC7 certification.
Rate: interval-average change in selected displacement quantity per elapsed day. Resultant rate is not vector speed. No forecast.
Report: editable draft evidence summary, not a completed ground-investigation report or approved design report. Summary ranges are descriptive and not design values.
No sample data are supplied. Empty views are intentional.
Data remain in the browser; the application makes no data-upload requests. This prototype has no access control, audit log, encryption service, persistent database or collaborative review workflow. Use only in accordance with your organisation's data policies.

Engineering background: Murakami et al. (2023), Developments of inverse analysis by Kalman filters and Bayesian methods applied to geotechnical engineering, https://pmc.ncbi.nlm.nih.gov/articles/PMC10749391/ . The dashboard does not implement these methods.
