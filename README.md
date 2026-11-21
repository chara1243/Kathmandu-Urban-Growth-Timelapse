# Kathmandu Urban Growth Timelapse (1950–2025)

A Python-based geospatial visualization project showing the spatial distribution and model-estimated expansion of buildings in Kathmandu, Nepal.

## Project Overview

This project uses OpenStreetMap building footprints and Python geospatial libraries to create an animated visualization of Kathmandu's urban expansion.

The workflow assigns estimated construction years using a distance-based spatial model and generates maps at two-year intervals from 1950 to 2025.

## Technologies

- Python
- GeoPandas
- OSMnx
- Matplotlib
- Contextily
- NumPy
- ImageIO
- Jupyter Notebook

## Project Workflow

1. Download building footprints from OpenStreetMap.
2. Clean and validate building geometries.
3. Project spatial data into UTM Zone 45N.
4. Calculate distances from the selected city centre.
5. Assign model-estimated construction years.
6. Generate spatial maps at two-year intervals.
7. Export animated GIF and MP4 files.

## Repository Structure

```text
notebooks/
    kathmandu_urban_growth.ipynb
outputs/
src/
README.md
requirements.txt
.gitignore
LICENSE
```

## Installation

Clone the repository:

```bash
git clone https://github.com/YOUR_USERNAME/Kathmandu-Urban-Growth-Timelapse.git
```

Navigate into the project:

```bash
cd Kathmandu-Urban-Growth-Timelapse
```

Install dependencies:

```bash
pip install -r requirements.txt
```

Launch Jupyter:

```bash
jupyter notebook
```

Open the notebook inside the notebooks folder and execute the cells.

## Outputs

The notebook generates:

- `kathmandu_timelapse.gif`
- `kathmandu_timelapse.mp4`
- Individual yearly map frames.

## Methodological Limitation

The assigned building construction years are simulated estimates based on distance from the selected city centre, with random variation and a simplified earthquake-related adjustment. They are not verified construction dates or historical building records.

The visualization should therefore be interpreted as a hypothetical spatial growth model rather than an empirical reconstruction of historical urban expansion.

## Data Source

Building footprint data are retrieved from OpenStreetMap.

© OpenStreetMap contributors.

https://www.openstreetmap.org/copyright

## Author

Charan Bhattarai

## License

This project is distributed under the MIT License.
