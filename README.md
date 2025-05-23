# Damien Hirst Dot Painting Generator

![Preview](docs/preview.png)

A lightweight Python Turtle script that recreates the look of Damien Hirst's iconic Spot paintings. Run the program and watch as a 10 x 10 grid of brightly coloured dots appears on your screen.

## Features

* Generates a grid of 100 dots using a hand‑picked palette
* Fully randomised colours per dot for endless variety
* Easy to adjust grid size, spacing and dot diameter

## Requirements

* Python 3.8 or newer
* Turtle graphics library (bundled with the standard Python build)
* No external dependencies

## Installation

```bash
git clone https://github.com/your-username/hirst-dot-generator.git
cd hirst-dot-generator
python main.py
```

If you are on macOS and use Homebrew Python you may need to install the native Tcl/Tk support to see the Turtle window:

```bash
brew install tcl-tk
```

## Usage

Open **main.py** and tweak the following variables if you want a custom canvas:

```python
color_list = [...]   # 34 RGB tuples you can replace or extend
grid_size = 10       # number of dots per row and column
spacing = 70         # distance in pixels between dots
dot_size = 20        # diameter of each dot
```

Then run

```bash
python main.py
```

Close the Turtle window when you are ready to exit.

## How it works

The script positions the Turtle cursor at the bottom left corner, then iterates across rows and columns. For each position it teleports the cursor and draws a filled circle (`turtle.dot`) with a randomly chosen colour from the palette.

## Contributing

Pull requests are welcome. Please open an issue first to discuss significant changes.

## License

This project is licensed under the MIT License. See **LICENSE** for details.
