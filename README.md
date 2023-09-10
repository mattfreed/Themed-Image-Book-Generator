# Poem Themed Image Book Generator

## Overview

This project is designed to automate the generation of a PDF book that pairs unique poem themes with corresponding images. The project consists of three primary stages:

1. Generating poem themes using OpenAI's GPT-3.5-turbo via the `ChatGPTThemeGenerator.ipynb` Jupyter Notebook.
2. Creating image prompts for the MidJourney software using the `MidJourneyPromptGenerator.ipynb` Jupyter Notebook.
3. Generating a PDF book that pairs the images with the poem themes using the `BookPDFGenerator.ipynb` Jupyter Notebook.

<img src="/GIF/ezgif.com-gif-maker.gif" width="400" class="center"/>

## Table of Contents

- [Requirements](#requirements)
- [Installation](#installation)
- [Usage](#usage)
- [File Structure](#file-structure)
- [How it Works](#how-it-works)
- [Contributing](#contributing)
- [License](#license)

## Requirements

* Python 3.6+
* Pandas
* PIL (Pillow)
* FPDF
* OpenAI Python package
* Jupyter Notebook

## Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/yourusername/yourrepository.git
    ```
    
2. Navigate to the directory:
    ```bash
    cd yourrepository
    ```

3. Install the required Python packages:
    ```bash
    pip install pandas Pillow fpdf openai notebook
    ```

4. Open Jupyter Notebook to view and run the notebooks:
    ```bash
    jupyter notebook
    ```

## Usage

1. Add your OpenAI API key in a file named `key.txt`.

2. Prepare the `Poems/Vol1`, `Images/Vol1`, and `Books` folders.

3. Run the notebooks in the following order:
    1. `ChatGPTThemeGenerator.ipynb` for generating poem themes.
    2. `MidJourneyPromptGenerator.ipynb` for generating image prompts.
    3. `BookPDFGenerator.ipynb` for creating the final PDF book.

This will generate a PDF book in the `Books` folder.

## File Structure

- `ChatGPTThemeGenerator.ipynb`: Jupyter Notebook for generating poem themes.
- `MidJourneyPromptGenerator.ipynb`: Jupyter Notebook for generating MidJourney image prompts.
- `BookPDFGenerator.ipynb`: Jupyter Notebook for generating the PDF book.
- `Poems/Vol1/poems_vol1.csv`: CSV file containing poem themes.
- `Images/Vol1`: Folder containing generated images.
- `Books`: Folder where the generated PDF will be saved.

## How it Works

1. **Fetching Poem Themes**: Utilizes GPT-3.5-turbo to generate a list of unique poem themes in `ChatGPTThemeGenerator.ipynb`.
2. **Image Generation Prompts**: Creates prompts for MidJourney to generate images based on the poem themes using `MidJourneyPromptGenerator.ipynb`.
3. **PDF Compilation**: Uses the FPDF library to compile the images and titles into a PDF in `BookPDFGenerator.ipynb`.

## Contributing

Feel free to fork the project and submit a pull request with your changes!

## License

MIT License. See `LICENSE` for more information.
