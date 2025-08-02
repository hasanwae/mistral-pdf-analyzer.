Mistral PDF Summarizer and QA Tool
This project provides a Python-based tool for summarizing PDF documents and answering questions about their content using the Mistral-7B-Instruct model from Hugging Face. It leverages a Gradio interface for user-friendly interaction, allowing users to upload PDF files, view summaries, and ask questions about the document content.
Features

PDF Text Extraction: Extracts text from uploaded PDF files using PyMuPDF.
Document Summarization: Generates concise summaries of PDF content using the Mistral-7B-Instruct model.
Question Answering: Answers user-specified questions based on the PDF content.
Interactive UI: Provides a web-based interface built with Gradio for easy file uploads and query inputs.
GPU Acceleration: Supports 4-bit quantization for efficient model loading and inference on compatible hardware.

Requirements

Python 3.8+
PyTorch
Transformers
Accelerate
BitsAndBytes
PyMuPDF
Gradio

Installation

Clone the repository:
git clone https://github.com/your-username/mistral-pdf-summarizer.git
cd mistral-pdf-summarizer


Install the required dependencies:
pip install -q transformers accelerate bitsandbytes PyMuPDF gradio


Ensure you have a Hugging Face token to access the Mistral model. Set it up when prompted by the script.


Usage

Run the Jupyter notebook Mistral_PDF_Summarizer_and_QA_Tool_ipynb_.ipynb or execute the script in a Python environment.
The Gradio interface will launch in your browser (or provide a public URL if running on Colab).
Upload a PDF file using the interface.
Enter a question about the PDF content (optional).
Click "Start analysis" to generate a summary and answer to your question.

Example

Upload a PDF document.
Ask a question like: "What is the main topic of the document?"
The tool will output a summary of the document and an answer to your question.

Notes

The tool uses 4-bit quantization to optimize performance on GPUs. Ensure you have a compatible GPU for faster inference.
A Hugging Face token is required to access the Mistral-7B-Instruct model.
The Gradio interface may require share=True when running on hosted environments like Colab.
For large PDFs, processing time may vary depending on the document length and hardware.

License
This project is licensed under the MIT License. See the LICENSE file for details.
Acknowledgments

Built using the Mistral-7B-Instruct-v0.1 model by Mistral AI.
Utilizes PyMuPDF for PDF text extraction and Gradio for the web interface.
