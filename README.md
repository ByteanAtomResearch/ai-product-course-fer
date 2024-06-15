
[![LinkedIn][linkedin-shield]][linkedin-url]
[![Youtube][youtube-shield]][youtube-url]
[![Udacity][udacity-shield]][udacity-url]

# LLM Fairness Evaluation Exercise - Mango Oasis Chatbot

[![Libraries Used](https://img.shields.io/badge/libraries-RAGAS%20%7C%20DeepEval-blue)](https://github.com/explodinggradients/ragas,https://github.com/deep-eval/deepeval)
[![Run in Google Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ByteanAtomResearch/ai-product-course-fer/blob/main/mangobot_fer.ipynb)

This exercise guides you through assessing the fairness of the Mango Oasis AI chatbot, with a focus on detecting and mitigating geographical bias in its responses. The output includes metric calculations, visualizations, and actionable recommendations.

## Goal

- Analyze chatbot responses for potential geographical biases.
- Calculate faithfulness, answer relevance, and bias metrics.
- Visualize results to understand the extent of bias.
- Provide recommendations to improve fairness.

## Requirements

- Python
- Pandas
- Matplotlib
- RAGAS
- DeepEval
- Seaborn

## Instructions

1. **Data Preparation:**
   - Ensure your data file (containing chatbot conversations) is in the correct format and accessible to the script.

2. **Running the Code:**
   - **Option 1: Google Colab (Recommended)**
     - Click the "Run in Google Colab" badge above.
     - Upload your data file to Colab.
   - **Option 2: Local Execution**
     - Ensure you have Python installed locally.
     - Modify library installations (change `!pip install` to `%pip install`).
     - Store secrets as environment variables using `os.environ.get("SECRET_NAME")`.

3. **Follow the Notebook:** 
   - The provided notebook (or script) will guide you through each step:
     - Loading the data
     - Calculating metrics (faithfulness, answer relevance, bias)
     - Detecting bias using the `create_test_cases` function
     - Visualizing results (answer relevance distribution)
     - Generating a report with your findings and recommendations

## Key Functions

- `create_test_cases(data)`: Converts your dataset into DeepEval's format for bias analysis.
- `visualize_answer_relevancy(relevancy_df)`: Generates a plot to visualize answer relevance score distribution.

## Customization

- Adapt the data loading process to your file structure.
- Modify the `threshold` in `BiasMetric` for bias sensitivity.
- Explore other fairness metrics in RAGAS and DeepEval.

## Notes

- The example plot visualizes answer relevance; create similar plots for other metrics.
- Dive into the resulting dataframes (`faithfulness_score_df`, `answer_relevance_df`, `geographical_bias_df`) for in-depth analysis.


## License

Distributed under the Apache License. See `LICENSE` for more information.
Copyright (c) 2024 Noble Ackerson

[linkedin-url]: https://linkedin.com/in/noblea
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
[youtube-url]: https://youtube.com/c/nobleackerson
[udacity-url]: https://www.udacity.com/course/ai-product-manager-nanodegree--nd088
[youtube-shield]: https://img.shields.io/badge/-Youtube-black.svg?style=for-the-badge&logo=youtube&colorB=555
[udacity-shield]: https://img.shields.io/badge/-Udacity-black.svg?style=for-the-badge&logo=udcaity&colorB=555
