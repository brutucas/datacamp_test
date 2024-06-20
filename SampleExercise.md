# Sample Exercise: Basic Text Generation with GPT-2

- This exercise demonstrates basic text generation using the GPT-2 model with the Hugging Face Transformers library. 
- Learners will load a pre-trained model and tokenizer, then complete a script that generates text based on a given input prompt. 
- Upon completion of this exercise, learners will have loaded a Hugging Face transformer model, generated text, and better understand parameters.

#### Instruction 1: Import the necessary libraries from Hugging Face
from transformers import 1)___ as

from transformers import 2)___ as

#### Instruction 2: Load the pre-trained model and tokenizer
model = 1)___ .from_pretrained('gpt2')

tokenizer = 2)___ .from_pretrained('gpt2')

#### Instruction 3: Encode some input text
inputs = tokenizer.encode("Today's weather is", add_special_tokens=True, return_tensors='pt')

#### Instruction 4: Generate text using the model
outputs = model.generate(inputs, max_length= 3)___ , num_return_sequences= 4)___)

print("Generated text:", tokenizer.decode(outputs[0], skip_special_tokens=True))

#### Here are the exercise instructions in different format:
- Replace 1)___ with the name of the class for loading the model.
  
- Replace 2)___ with the name of the tokenizer class from the Transformers library.
  
- Fill in 3)___ to set the number of tokens for the generated text as 50.
  
- Input a suitable number in 4)___ to generate 2 different text sequences based on the input.
  
- BONUS: Run the code with various inputs and parameters and consider the impact on generated text output with changes in max_length and num_return_sequences.

Answers:
1) GPT2LMHeadModel
2) GPT2Tokenizer
3) 50
4) 2
