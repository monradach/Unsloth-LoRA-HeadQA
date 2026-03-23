**HEAD-QA Fine-Tuning with Llama 3.2**

This repository is a small introductory project using Unsloth to fine-tune Llama 3.2 on the HEAD-QA medical multiple-choice QA dataset. For this purpose, only 5,000 samples were used across training and testing to keep the workflow lightweight and easy to run.

The project covers basic dataset preprocessing, chat-template formatting, response-only supervised fine-tuning, and simple test-set evaluation with accuracy. Its goal is to provide a compact starting point for learning how to use Unsloth for medical QA fine-tuning.

## Results
This initial experiment was run on a small subset of **5,000 samples** to keep training lightweight.

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

## Model
The final model can be found on Hugging Face: https://huggingface.co/monradach/Llama-3.2-3B-Instruct-HeadQA
