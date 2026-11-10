PoseHarvest-and-Normalize-CSVJSON

Tiny prototype that demonstrates harvesting time-series/pose-like data from: CSV, JSON, and JPEG images (extracting EXIF DateTime and Orientation). Normalizes into a simple CSV and JSON schema for replay/trajectory analysis.

How to use
- Open index.html in a modern browser.
- Drag or select files: .csv, .json, .jpg/.jpeg
- The UI will parse and show normalized records and let you download normalized CSV/JSON.

Notes
- This is a minimal, client-side prototype (no network). It extracts basic EXIF fields only (DateTime, Orientation). More fields and bulk harvesting from websites require additional code and permissions.
- Schema: records have id, timestamp (ISO 8601 or empty), source_filename, type (csv/json/image), and pose.* fields if present (x,y,z,yaw,pitch,roll) or exif.orientation.

License: public demo for project use.