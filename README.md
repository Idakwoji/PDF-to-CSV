# PDF-to-CSV
## Upwork task
- The task here capitalizes on the back-end of the web application I already built that converts text-based and image-based pdfs to editable word documents OCR.
- The specific pdf data for this project was in a tabular format and it wouldve been difficult and more expensive to try to extract the tabular data.
- Using the tabular-py library would not yield results as this was an image-based pdf in which the tables were photographed from a physical paper.
- I decided that the most feasible approach would be to use my OCR exraction technique to convert the tables to text.
- The data in the text was in a semi-structured format, and required some cleaning, inspection, and the use of techniques such as regular expressions and various iterations to extract the data required by the client.
- Given that OCR is still relatively imperfect, some of the data (especially the "IDs") were inaccurate because the original pdf file had some blurry pages.
- I attempted to enhance the images gotten from the PDF during the OCR process by adjustig the sharpness and contrast using the "ImageEnhance" module from the Pillow library. This helped to greatly improve the accuracy of the text data (especially the IDs) and generally improved the output CSV file.
- I plan to integrate this image enhancement technique into my already hosted back-end as well, because it would generally improve the accuracy and reliabiliity of the project.
- Unfortunately, the client was lookign for perfection however, which was impossible to achieve given the time constraint of two days and the very low budget of the client.
- A solution I suggested to him was to use the OpenAI model to predict and improve the output extracted text by making corrections to the words that may come out distorted. Unfortunately, his budget could not cover the costs of making use of the model.
