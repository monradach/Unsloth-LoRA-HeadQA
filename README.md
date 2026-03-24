# HEAD-QA LoRA Fine-Tuning with Llama 3.2

This repository is a small introductory project showing how to use **Unsloth** to **LoRA fine-tune Llama 3.2** on the **HEAD-QA** medical multiple-choice QA dataset.

To keep the workflow lightweight and easy to run, the experiment uses **5,000 samples** in total, split into training and testing. The project demonstrates a simple end-to-end pipeline for:
- preprocessing the dataset
- formatting examples with a chat template
- applying response-only supervised fine-tuning
- evaluating performance with test accuracy

## Results

This experiment was run on a small subset of **5,000 samples**.

<table>
  <tr>
    <td valign="top">
      <table>
        <tr><th>Split</th><th>Size</th></tr>
        <tr><td>Train</td><td>4,000</td></tr>
        <tr><td>Test</td><td>1,000</td></tr>
      </table>
    </td>
    <td valign="top">
      <table>
        <tr><th>Metric</th><th>Score</th></tr>
        <tr><td>Accuracy</td><td>0.6340</td></tr>
      </table>
    </td>
  </tr>
</table>

> **Note:** The reported result is not directly comparable to the official HEAD-QA baselines, since this project uses only a small unstratified subset rather than the benchmark’s original split.

## Model

Available on Hugging Face: [monradach/Llama-3.2-3B-Instruct-HeadQA](https://huggingface.co/monradach/Llama-3.2-3B-Instruct-HeadQA)
