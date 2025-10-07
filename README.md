# GPT-2 Playground (2019)

> **About this fork**
>
> This fork adds a simple, no-code **chat interface** for GPT-2 — one of the earliest ways to talk to a large language model, before ChatGPT existed.
>  
> Built as a **Google Colab notebook**, it allowed anyone to spin up GPT-2 in minutes without installation or programming, helping popularize hands-on experimentation with LLMs.  
>  
> Created by **Ignacio G. López-Francos**, later featured in *The Economist*’s “The World in 2020” special edition.

[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ilopezfr/gpt-2/blob/master/gpt-2-playground_.ipynb)

---

## GPT-2 Playground

A browser-based, interactive chat notebook for experimenting with GPT-2 models released by OpenAI.

**Features**
- **Zero setup:** open the notebook in Colab, press *Run all*, and start chatting.
- **Accessible:** designed for non-coders, with clear cell annotations and UI prompts.
- **Configurable:** choose model size (small–XL), adjust sampling parameters (`temperature`, `top-k`, `top-p`), and set custom prompts.
- **Reproducible:** runs entirely from this repository with pinned dependencies inside the notebook.

**Quick Start**
1. Click the *Open in Colab* badge above.  
2. In Colab, choose **Runtime → Run all**.  
3. Select a model size and start interacting with GPT-2 in the chat cell.  

> *Tip:* Free Colab GPUs handle up to the 774M model comfortably; the 1.5B model may require Colab Pro or a local GPU runtime.

---
# Original OpenAI README (unchanged)

**Status:** Archive (code is provided as-is, no updates expected)

# gpt-2

Code and models from the paper ["Language Models are Unsupervised Multitask Learners"](https://d4mucfpksywv.cloudfront.net/better-language-models/language-models.pdf).

You can read about GPT-2 and its staged release in our [original blog post](https://blog.openai.com/better-language-models/), [6 month follow-up post](https://openai.com/blog/gpt-2-6-month-follow-up/), and [final post](https://www.openai.com/blog/gpt-2-1-5b-release/).

We have also [released a dataset](https://github.com/openai/gpt-2-output-dataset) for researchers to study their behaviors.

<sup>*</sup> *Note that our original parameter counts were wrong due to an error (in our previous blog posts and paper).  Thus you may have seen small referred to as 117M and medium referred to as 345M.*

## Usage

This repository is meant to be a starting point for researchers and engineers to experiment with GPT-2.

For basic information, see our [model card](./model_card.md).

### Some caveats

- GPT-2 models' robustness and worst case behaviors are not well-understood.  As with any machine-learned model, carefully evaluate GPT-2 for your use case, especially if used without fine-tuning or in safety-critical applications where reliability is important.
- The dataset our GPT-2 models were trained on contains many texts with [biases](https://twitter.com/TomerUllman/status/1101485289720242177) and factual inaccuracies, and thus GPT-2 models are likely to be biased and inaccurate as well.
- To avoid having samples mistaken as human-written, we recommend clearly labeling samples as synthetic before wide dissemination.  Our models are often incoherent or inaccurate in subtle ways, which takes more than a quick read for a human to notice.

### Work with us

Please [let us know](mailto:languagequestions@openai.com) if you’re doing interesting research with or working on applications of GPT-2!  We’re especially interested in hearing from and potentially working with those who are studying
- Potential malicious use cases and defenses against them (e.g. the detectability of synthetic text)
- The extent of problematic content (e.g. bias) being baked into the models and effective mitigations

## Development

See [DEVELOPERS.md](./DEVELOPERS.md)

## Contributors

See [CONTRIBUTORS.md](./CONTRIBUTORS.md)

## Citation

Please use the following bibtex entry:
```
@article{radford2019language,
  title={Language Models are Unsupervised Multitask Learners},
  author={Radford, Alec and Wu, Jeff and Child, Rewon and Luan, David and Amodei, Dario and Sutskever, Ilya},
  year={2019}
}
```

## Future work

We may release code for evaluating the models on various benchmarks.

We are still considering release of the larger models.

## License

[Modified MIT](./LICENSE)
