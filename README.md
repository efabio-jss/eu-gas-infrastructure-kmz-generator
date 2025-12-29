# 🌍 Gas Infrastructure KMZ Generator
An automated tool to convert GeoJSON layers of gas infrastructure into a styled KMZ file for visualization in Google Earth.

📘 Overview
This repository provides a Python script that:

Reads GeoJSON files extracted from entsog.eu representing nodes, pipelines, production sites, and storage facilities.
Infers node types based on names and applies custom icons.
Generates a KMZ file with styled points and lines for easy visualization.

Ideal for energy infrastructure mapping and geospatial analysis.

✅ Features

Supports multiple layers: Nodes, PipeSegments, Productions, Storages.
Custom icons per node type:

Storage, Production, Entry/Exit Points, LNG Terminal, Compressor Station, Interconnection Point.


Styled lines for pipelines (neon purple, width 3).
Rich metadata pop-ups with:

ID, Name, Country, Type, Status, Commissioning/Decommissioning years.


Handles param and method fields as JSON for detailed attributes.

⚙️ Technology Stack

Python

geopandas
simplekml
json (built-in)
os (built-in)

▶️ How It Works

Load GeoJSON layers using GeoPandas.
Infer node type from the name field.
Apply styles:

Points → custom icons + neon blue color.
Lines → neon purple color + width 3.


Generate KMZ using simplekml and save to the specified folder.

🏁 Final Notes
This tool simplifies the process of converting raw geospatial data into a visual KMZ map for energy infrastructure projects. Perfect for analysts, engineers, and GIS professionals.
