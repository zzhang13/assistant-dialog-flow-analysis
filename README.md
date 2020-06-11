# Watson Assistant Dialog Flow Analysis

> Note: help us stay in touch and improve this notebook by clicking on the :star: star icon (top right).

This repository hosts the the Watson Assistant Dialog Flow Analysis Notebook and the underlying conversation analytics toolkit library.

<details>
 <summary>Table of Contents</summary>

 
 [Introduction](#introduction)<br>
 [Getting Started](#getting-started)<br>
 [Guides](#guides)<br>
 [Frequently Asked Questions](#frequently-asked-questions)<br>
 [License](#license)<br>
 [Contributing](#contributing)<br>

</details>

## Introduction

The Watson Assistant Dialog Flow Analysis Notebook can help you assess and analyze user journeys and issues related to the dialog flow of ineffective (low quality) conversations based on production logs.  The notebook can help you with questions such as:
- What are the common conversation steps and flows within the assistant 
- Which flows have low task completion rates and high abandonment (ineffective conversations)
- Where along the dialog steps users lose engagement with your assistant
- What are common terms and steps that may lead to abandonment

This notebook extends the [Measure and Analyze notebooks](https://github.com/watson-developer-cloud/assistant-improve-recommendations-notebook) by providing additional capabilities to assess and analyze effectiveness - focused more on issues related to the dialog flow.  For more details, check out [IBM Watson Assistant Continuous Improvement Best Practices](https://github.com/watson-developer-cloud/assistant-improve-recommendations-notebook/raw/master/notebook/IBM%20Watson%20Assistant%20Continuous%20Improvement%20Best%20Practices.pdf).


<img src="./notebooks/images/flow-vis.png" width="50%">

## Getting Started

The notebook requires a Jupyter Notebook environment and Python 3.6+.   You can either install Jupyter Notebook to run locally or you can use Watson Studio on the cloud.

### Using Jupyter Notebook
1. Install Python 3.6+
2. Install Jupyter notebook. Checkout the [Jupyter/IPython Notebook Quick Start Guide](https://jupyter-notebook-beginner-guide.readthedocs.io/en/latest/install.html) for more details
3. Download the `notebooks/Dialog Flow Analysis Notebook.ipynb` file.   
4. Start jupyter server `jupyter notebook`
5. Run the `Dialog Flow Analysis Notebook.ipynb`

### Using Watson Studio
1. Create a new custom runtime environment.  Select Python 3.6+ as the base.  In the customization section pane, update the list of dependencies as defined in [requirements.txt](./requirements.txt).
```
dependencies:
  - pip:
    - pandas~=0.24.0
    - textblob>=0.15.3
    - scikit-learn>=0.21.3
    - scipy>=1.3.0
    - numpy>=1.15.4
    - requests>=2.18.4
    - nltk>=3.4.5
    - ibm-watson>=4.3.0
    - tqdm>=4.31.1
    - plotly>=4.5.0
```
2. Select `Add to Project`-->`Notebook`.  Choose `From URL` and paste this [url](https://raw.githubusercontent.com/watson-developer-cloud/assistant-dialog-flow-analysis/master/notebooks/Dialog%20Flow%20Analysis%20Notebook.ipynb).  Alternately you can select `From file` and upload the `notebooks/Dialog Flow Analysis Notebook.ipynb` file.
3. Run the notebook using the newly created runtime environment (note: the first time use of the runtime environment, can take a few minutes to prepare)

## Guides
Coming soon...

## Frequently Asked Questions
See [FAQ.md](FAQ.md) for frequently asked questions 

## License
This library is licensed under the [Apache 2.0 license](http://www.apache.org/licenses/LICENSE-2.0).

## Contributing 
See [CONTRIBUTING.md](CONTRIBUTING.md) and [DEVELOPER.MD](DEVELOPER.MD) for more details on how to contribute
