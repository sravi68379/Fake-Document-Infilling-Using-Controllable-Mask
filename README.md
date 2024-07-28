Project Overview
This project focuses on creating fake document infilling using controllable masking for cyber deception. By leveraging a trained BERT model, the system generates believable but false alternatives for masked sensitive data, enhancing cybersecurity through data obfuscation.

Key Features
Random Masking and Training: Performed random masking on sensitive data (e.g., patent data) and trained a BERT model on this masked data.
Importance Score Calculation: Used the RAKE algorithm to calculate the importance score of new sensitive documents, guiding the masking process.
Controllable Masking: Applied controllable masking based on the calculated importance scores to strategically mask important concepts.
Penalization Decoding: Implemented penalization decoding during infilling to ensure the generated words are plausible but false alternatives.

Results
The generated documents contain believable but false alternatives to the masked sensitive data, providing an effective method for cyber deception.


Contact
For any questions or inquiries, please contact sravi68379@gmail.com.






Library Required:

import transformers (version==4.40.2)
import tensorflow as tf (version==2.15.0)
from transformers import BertTokenizer, TFBertForMaskedLM
import os
import numpy as np (version== 1.25.2)
import re (version==2.2.1)
import matplotlib.pyplot as plt
import random
from rake_nltk import Rake (version==3.8.1)



System Requirements:

Operating System:
	•	Windows 10 (or later)
	•	macOS Monterey (or later)
	•	Linux Ubuntu 22.04 (or later) (other LTS versions may also work)
Python Version:
	•	Python 3.10 or higher 
Hardware:
	•	Recommended: A computer with a dedicated GPU (Graphics Processing Unit) with at least 8GB of memory will accelerate training times.
	•	Minimum: A CPU with a decent amount of RAM (at least 16GB) can be used for training on smaller datasets or for inference


Saved Trained ModelModel Link= https://drive.google.com/file/d/1-jIxSerhmkCD8zz5IgkTyIducEmr-Z_8/view?usp=sharing
