# Sample Exercise: Basic Text Generation with GPT-2

- This exercise demonstrates basic text generation using the GPT-2 model with the Hugging Face Transformers library. 
- Learners will load a pre-trained model and tokenizer, then complete a script that generates text based on a given input prompt. 
- Upon completion of this exercise, learners will have loaded a Hugging Face transformer model, generated text, and better understand parameters.
***
#### Instructions:
- Import `GPT2LMHeadModel` and `GPT2Tokenizer` from the `transformers` library.
- Load the model and tokenizer from `.pretrained` 
- Set the number of tokens for the `max_length` of generated text as 50.
- Generate 2 different text sequences with `num_return_sequences` input.
  
- BONUS: Run the code with various inputs and parameters and consider the impact on generated text output with changes in `max_length` and `num_return_sequences`.
***
```python
# Import the necessary libraries from Hugging Face
from transformers import ____ as ____ # gpt2 model
from transformers import ____ as ____ # tokenizer

# Load the pre-trained model and tokenizer
model = ____.from_pretrained('gpt2') 
tokenizer = ____.from_pretrained('gpt2')

# Encode some input text
inputs = tokenizer.encode("Today's weather is", add_special_tokens=True, return_tensors='pt')

# Generate text using the model
outputs = model.generate(inputs, max_length=____, num_return_sequences=____)
print("Generated text:", tokenizer.decode(outputs[0], skip_special_tokens=True))
```
***
<details>
<summary>Hints:</summary>
<br>
Welcome to this very extravagant dropdown.
  <br>
In a more complicated exercise, I would include the hints here.
</details>

***

<details>
<summary>Answers:</summary>
<br>
1) GPT2LMHeadModel
  <br>
2) GPT2Tokenizer
  <br>
3) 50
  <br>
4) 2
</details>

