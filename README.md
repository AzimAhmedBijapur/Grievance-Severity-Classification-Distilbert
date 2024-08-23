# Fine-tuned distilbert for classifying complaints by severity (low, medium, high)

## Deployment link
https://huggingface.co/azim17/Gbert-85

## Use a pipeline as a high-level helper
from transformers import pipeline <br/>
pipe = pipeline("text-classification", model="azim17/Gbert-85") 

## Load model directly
from transformers import AutoTokenizer, AutoModelForSequenceClassification <br/>
tokenizer = AutoTokenizer.from_pretrained("azim17/Gbert-85") <br/>
model = AutoModelForSequenceClassification.from_pretrained("azim17/Gbert-85")
