ReverSea

ReverSea is a lightweight, depth-aware CNN for enhancing low-light underwater images. It directly processes raw images by incorporating transmission maps to restore natural colors, improve visibility, and handle non-uniform illumination.

Highlights

No preprocessing required

Depth-aware enhancement using transmission maps

Lightweight CNN architecture

Effective in deep-sea and low-light conditions

Block Diagram

Installation and Setup
Clone the Repository
git clone https://github.com/AIRLabIISc/REVERSEA.git
cd REVERSEA

Create a Virtual Environment (Recommended)

ReverSea was tested using Python 3.12. Creating a virtual environment is recommended.

python3.12 -m venv reversea
source reversea/bin/activate   # Linux / macOS
# reversea\Scripts\activate    # Windows

Install Dependencies

All required dependencies are listed in requirements.txt.

pip install --upgrade pip
pip install -r requirements.txt

Pretrained Weights

The weights/ directory contains pretrained models for different datasets.
Each dataset has its own dedicated folder.

SeaThru Dataset Weights
weights/SeaThru/


https://github.com/AIRLabIISc/REVERSEA/tree/main/weights/SeaThru

OceanDark Dataset Weights
weights/OceanDark/


https://github.com/AIRLabIISc/REVERSEA/tree/main/weights/OceanDark

Ensure the folder structure is preserved exactly as provided.

Training and Inference

Both training and inference are handled using a single notebook.

train+inf.ipynb


Open the notebook and run all cells to:

Train the model

Perform inference

Evaluate results

No separate preprocessing steps are required; the model directly operates on raw underwater images using transmission maps.

Paper

ReverSea: A Depth-Aware CNN for Low-Light Underwater Image Enhancement
https://ieeexplore.ieee.org/abstract/document/11104786

Citation
@inproceedings{makam2025reversea,
  title={ReverSea: An Enhancement Technique for Low-Lit Underwater Images},
  author={Makam, Rajini and Shankari, Dhatri and Patil, Sharanya and Sundram, Suresh},
  booktitle={OCEANS 2025 Brest},
  pages={1--8},
  year={2025},
  organization={IEEE}
}
