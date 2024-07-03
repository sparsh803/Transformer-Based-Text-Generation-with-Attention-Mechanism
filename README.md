<!-- Improved compatibility of back to top link: See: https://github.com/othneildrew/Best-README-Template/pull/73 -->
<a name="readme-top"></a>

## Table Of Contents
<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li><a href="#about-the-project">About The Project</a>
      <ul>
        <li><a href="#understanding-transformer-and-attention">Understanding Transformer and Attention Mechanism</a></li>
      </ul>
    </li>
    <li><a href="#implementation-details">Implementation Details</a>
      <ul>
        <li><a href="#model-architecture">Model Architecture</a></li>
        <li><a href="#training-the-model">Training the Model</a></li>
        <li><a href="#text-generation">Text Generation</a></li>
      </ul>
    </li>
    <li><a href="#built-with">Built With</a></li>
    <li><a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#installation">Installation</a></li>
        <li><a href="#step-by-step-guide">Step-by-Step Guide</a></li>
      </ul>
    </li>
    <li><a href="#contact">Contact</a></li>
  </ol>
</details>

<!-- ABOUT THE PROJECT -->
## About The Project
<a id="about-the-project"></a>

This project explores the implementation of a Generative Pre-trained Transformer (GPT) model from scratch. This model leverages the power of transformer architecture, specifically designed to handle sequential data while incorporating attention mechanisms for enhanced performance in natural language processing tasks.

### Understanding Transformer and Attention Mechanism
<a id="understanding-transformer-and-attention"></a>
The Transformer architecture revolutionized NLP by introducing a mechanism that allows capturing relationships between words in a sequence without the need for recurrent or convolutional layers. The Transformer model relies on self-attention mechanisms, which enable it to weigh the importance of different words in a sequence dynamically. This capability significantly improves the model's ability to understand context and dependencies within a text.

## Implementation Details
<a id="implementation-details"></a>

### Model Architecture
<a id="model-architecture"></a>

The GPT model implemented in this project leverages the Transformer architecture, integrating multiple layers of self-attention and feedforward neural networks. Each attention head in the model learns distinct relationships between words, collectively enhancing the model's comprehension of language patterns and semantics. This enables the model to generate coherent and contextually relevant text sequences autonomously.


### Training the Model
<a id="training-the-model"></a>
The loss function loss_fn computes the Cross Entropy Loss between predicted logits and targets. It reshapes logits and targets to facilitate computation and ensure consistency across batch dimensions, aiming to minimize the discrepancy between predicted and actual outputs during model training.
Training the GPT model involves iterating through Config.train_iters batches. Each batch consists of inputs and corresponding targets fetched from the training dataset (train_ds). Logits are computed using the model, and a loss function (loss_fn) evaluates the difference between predicted and actual targets. The optimizer updates model parameters based on computed gradients, aiming to minimize the loss and improve model performance.

### Text Generation
<a id="text-generation"></a>

Once trained, the GPT model demonstrated its capability to generate text autonomously. This involved providing an initial prompt or seed text to the model, which then utilized its learned parameters and attention mechanisms to predict the subsequent tokens in the sequence. The generated text reflects the model's understanding of language structure and semantics based on its training on a corpus of text data.

<p align="right">(<a href="#readme-top">back to top</a>)</p>


<!-- BUILT WITH -->
## Built With
<a id="built-with"></a>

* [Python](https://www.python.org/) - Programming Language
* [PyTorch](https://pytorch.org/) - Deep Learning Framework
* [dataclasses](https://docs.python.org/3/library/dataclasses.html) - Data Structures Library
* [Pathlib](https://docs.python.org/3/library/pathlib.html) - File System Paths Library

<p align="right">(<a href="#readme-top">back to top</a>)</p>


<!-- GETTING STARTED -->
## Getting Started
<a id="getting-started"></a>

### Installation
<a id="installation"></a>

Install the required libraries using the following markdown:

```markdown
- `pip install torch torchvision`
- `pip install tqdm`
- `pip install dataclasses`
- `pip install pathlib`
```

Ensure all libraries are installed before proceeding with the setup on Kaggle.
<p align="right">(<a href="#readme-top">back to top</a>)</p>

Follow these steps to get started with the project on Kaggle:
Step-by-Step Guide

<a id="step-by-step-guide"></a>

    Download the Notebook:
        Download the Jupyter Notebook (*.ipynb) from the GitHub repository.

    Upload to Kaggle:
        Click on "New Notebook" and choose the option to upload the notebook file.

    Set the Accelerator:
        Once the notebook is uploaded, go to the "Settings" tab.
        Under "Accelerator", select "GPU (P100)" to utilize Kaggle's high-performance GPU for faster computation.

    Run the Notebook:
        Save the settings and run the notebook to train and test your deep learning model.
        Monitor the progress and results directly within the Kaggle notebook environment.

<!-- CONTACT -->

<a id="contact"></a>
Contact

Sparsh Gupta - sparshg2003@gmail.com

Project Link: https://github.com/sparsh803/Transformer-Based-Text-Generation-with-Attention-Mechanism
<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[contributors-shield]: https://img.shields.io/github/contributors/othneildrew/Best-README-Template.svg?style=for-the-badge
[contributors-url]: https://github.com/othneildrew/Best-README-Template/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/othneildrew/Best-README-Template.svg?style=for-the-badge
[forks-url]: https://github.com/othneildrew/Best-README-Template/network/members
[stars-shield]: https://img.shields.io/github/stars/othneildrew/Best-README-Template.svg?style=for-the-badge
[stars-url]: https://github.com/othneildrew/Best-README-Template/stargazers
[issues-shield]: https://img.shields.io/github/issues/othneildrew/Best-README-Template.svg?style=for-the-badge
[issues-url]: https://github.com/othneildrew/Best-README-Template/issues
[license-shield]: https://img.shields.io/github/license/othneildrew/Best-README-Template.svg?style=for-the-badge
[license-url]: https://github.com/othneildrew/Best-README-Template/blob/master/LICENSE.txt
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
[linkedin-url]: https://linkedin.com/in/othneildrew
[product-screenshot]: images/screenshot.png
[Next.js]: https://img.shields.io/badge/next.js-000000?style=for-the-badge&logo=nextdotjs&logoColor=white
[Next-url]: https://nextjs.org/
[React.js]: https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB
[React-url]: https://reactjs.org/
[Vue.js]: https://img.shields.io/badge/Vue.js-35495E?style=for-the-badge&logo=vuedotjs&logoColor=4FC08D
[Vue-url]: https://vuejs.org/
[Angular.io]: https://img.shields.io/badge/Angular-DD0031?style=for-the-badge&logo=angular&logoColor=white
[Angular-url]: https://angular.io/
[Svelte.dev]: https://img.shields.io/badge/Svelte-4A4A55?style=for-the-badge&logo=svelte&logoColor=FF3E00
[Svelte-url]: https://svelte.dev/
[Laravel.com]: https://img.shields.io/badge/Laravel-FF2D20?style=for-the-badge&logo=laravel&logoColor=white
[Laravel-url]: https://laravel.com
[Bootstrap.com]: https://img.shields.io/badge/Bootstrap-563D7C?style=for-the-badge&logo=bootstrap&logoColor=white
[Bootstrap-url]: https://getbootstrap.com
[JQuery.com]: https://img.shields.io/badge/jQuery-0769AD?style=for-the-badge&logo=jquery&logoColor=white
[JQuery-url]: https://jquery.com 
