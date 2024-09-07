# Arabic-NLP-Generating-Multiple-Choice-Questions-of-Saudi-Schoolbooks
Our project in the Kaust Academy summer program in Artificial intelligence

The project  aims to leverage Natural Language Processing (NLP) to automate the creation of multiple-choice questions (MCQs) from Arabic texts in Saudi schoolbooks. The project addresses a key challenge in Arabic NLP, as Arabic is a morphologically rich and complex language, making it harder to process.
Input (Saudi Schoolbooks): The system takes Arabic schoolbooks in PDF format as input, but since these books are not machine-readable, extracting text directly from the PDFs is not feasible.

1- Text Extraction: A YOLOv5 model is used to extract paragraphs as images from the schoolbooks. These paragraph images are then passed through an Optical Character Recognition (OCR) model to convert the images into machine-readable text.

2- Text Processing (Chunking): The extracted text undergoes chunking, which involves cleaning and organizing the text into meaningful segments. These chunks represent important information from the book.

3-Text Alignment with Knowledge Dataset: The chunks are analyzed and matched with items from a general knowledge dataset to identify relevant content for generating questions.

4- Question Generation (RAG Approach): Using a Retrieval-Augmented Generation (RAG) approach, the aligned text and dataset information are used in prompts to generate questions.

6- MCQ Generation with GPT-4: The system finally employs a language model (GPT-4 or a smaller version) to generate multiple-choice questions based on the prompts.

The system aims to assist school teachers by reducing their workload in exam preparation and contributes to Arabic NLP advancements, supporting Saudi Vision 2030. The full report and project details can be found in the project documentation
