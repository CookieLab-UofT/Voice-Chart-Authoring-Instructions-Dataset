# Voice Chart-Authoring Instructions Dataset (VCAID)

Spoken chart-authoring instructions dataset from this CHI'24 Late-Breaking Work [paper](https://arxiv.org/abs/2404.05103).

## Citation

To credit this dataset, please cite our paper, "Chart What I Say: Exploring Cross-Modality Prompt Alignment in AI-Assisted Chart Authoring":
Nazar Ponochevnyi and Anastasia Kuzminykh. 2024

```bibtex
@inproceedings{Ponochevnyi2024Chart,
  author = {Ponochevnyi, Nazar and Kuzminykh, Anastasia},
  title = {Chart What I Say: Exploring Cross-Modality Prompt Alignment in AI-Assisted Chart Authoring},
  year = {2024},
  isbn = {9798400703317},
  publisher = {Association for Computing Machinery},
  address = {New York, NY, USA},
  url = {https://doi.org/10.1145/3613905.3650921},
  doi = {10.1145/3613905.3650921},
  booktitle = {Extended Abstracts of the 2024 CHI Conference on Human Factors in Computing Systems},
  articleno = {72},
  numpages = {7},
  keywords = {data visualization, natural language corpus, natural language interface, visualization authoring, visualization specification, voice interface},
  series = {CHI EA '24}
}
```

## Abstract

Recent chart-authoring systems, such as Amazon Q in QuickSight and Copilot for Power BI, demonstrate an emergent focus on supporting natural language input to share meaningful insights from data through chart creation. Currently, chart-authoring systems tend to integrate voice input capabilities by relying on speech-to-text transcription, processing spoken and typed input similarly. However, cross-modality input comparisons in other interaction domains suggest that the structure of spoken and typed-in interactions could notably differ, reflecting variations in user expectations based on interface affordances. Thus, in this work, we compare spoken and typed instructions for chart creation. Findings suggest that while both text and voice instructions cover chart elements and element organization, voice descriptions have a variety of command formats, element characteristics, and complex linguistic features. Based on these findings, we developed guidelines for designing voice-based authoring-oriented systems and additional features that can be incorporated into existing text-based systems to support speech modality.

## Dataset Overview

The Voice Chart-Authoring Instructions Dataset (VCAID) is contained within the [`VCAID.xlsx`](VCAID.xlsx) file. This dataset is designed to assist in analyzing the differences between spoken and typed instructions for chart creation, particularly focusing on the linguistic characteristics of voice-based instructions. The dataset is structured into two sheets:

### Instructions Sheet

This sheet contains 76 spoken instructions provided by 25 participants and the corresponding code snippets manually created by 2 researchers. The columns in this sheet are:

- **Text**: The text number used as scenario-based stimuli for each instruction (see the Texts Sheet for details).
- **Instruction**: The exact spoken instructions given by participants.
- **Code**: The Python code to create the chart described by the instruction, using libraries such as Plotly and NumPy.

### Texts Sheet

This sheet contains 8 scenario-based stimuli shown to participants in the data collection process. Its content is stored in a JSON-like structure.

## Data Usage

Researchers and developers can use this dataset to explore the linguistic structures of voice-based chart authoring instructions, compare them with typed instructions, and develop or refine systems that support voice-driven chart creation. The dataset provides valuable insights for designing voice interfaces that align more closely with user expectations and natural language use.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
