# Travel Pins Map

An interactive map to track places you have visited or want to visit, built using `ipyleaflet` and `ipywidgets` in Python. Pins can be added, updated, and deleted directly on the map, with persistent storage in a JSON file.

## Features

- Add pins on the map in **Add Pin** mode.  
- Each pin has a **name** and **status** ("Visited" or "Want to visit").  
- Click on a pin to **update**, **delete**, or **cancel** changes.  
- Pins are saved to a local JSON file (`travel_pins.json`).  
- Legend shows color coding for pin statuses.  
- Log output displays actions performed (add/update/delete/save).

## Installation

bash
pip install ipyleaflet ipywidgets

Note: Make sure you are using a Jupyter environment (Notebook or Lab) to run the map.

## Usage

Clone the repository.

Open the notebook containing the code.

Use the ➕ Add Pin button to enable pin placement on the map.

Click an existing pin to edit or delete it.

Use Save pins to file button to store changes in travel_pins.json.

## Color Legend

Red: Visited

Green: Want to visit

## How It Works

Pins are represented as CircleMarkers on an ipyleaflet map.

A MarkerCluster is used to manage multiple pins efficiently.

Pin data is loaded from and saved to a JSON file, allowing persistence between sessions.

Clicking on a pin opens an interactive popup with controls for editing.

Map interactions are handled using on_interaction events.

## Next Steps

Add filtering or search functionality.

Customize marker icons or sizes.

Integrate with an online backend for multi-user access.

Enable importing/exporting pin data.
