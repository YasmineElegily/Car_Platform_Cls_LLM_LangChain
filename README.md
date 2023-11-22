# Car_Platform_VGG19_LLM_LangChain
Improving our online car-selling platform by allowing users to add cars with images, text descriptions, and prices for a more convenient selling experience.

##	Solution Design Diagram
![image](https://github.com/YasmineElegily/Car_Platform_Cls_LLM_LangChain/assets/69461886/d2417204-e8a9-4808-aabd-a83f5c5e3364)

## 	Car Images data versions and classification model:
	* Link to the original data: "https://drive.google.com/file/d/1gibdLQwr8JkgTy2ek_pvK3_xF6ZbytaE/view?usp=sharing" 
	* Link to the resampled data: "https://drive.google.com/file/d/1-xcNvK21bjEHE087EgpvntJ2BYd7UnJR/view?usp=drive_link" 
	* Link to the model: "https://drive.google.com/file/d/1pCeCjFwNQxPW3U2SR_j9n7SB9-BBJWLW/view?usp=drive_link"


##	Car image classification Model:
After observing the data and reading the data_info.txt file about it I noticed very small classes like 'Van', 'Wagon' & 'Minivan'.
So I decided to do:
1) Data Augmentation
2) Weighting Classes in the model training
3) Fine-Tuning a Pre-trained Model
4) Drop-out and Kernel Regularization to decrease overfitting\
 *More approaches I tried to mitigate huge data imbalance*:\
6) Try the Focal Loss Function
7) Try LearningRateScheduler
8) Ensemble modeling
9) Re-weighting Classes
10) Resample the lowest classes on Roboflow.


##	Demo Instructions:
- To run the LLM and LangChain Test, You need to make a config_file.json for the sensitive data (OpenAI_API_Key) to not be exposed.

**To run the Car_Selling_Platform_Gradio_Demo, you need:**

1) Pre-trained Car Classification Saved Model that I uploaded to my Google Drive
	* Link to the model: "https://drive.google.com/file/d/1pCeCjFwNQxPW3U2SR_j9n7SB9-BBJWLW/view?usp=drive_link"
2) Label Encoder
	* I uploaded the label encoder to the Repo
3) Your "OPENAI_API_KEY" stored safely in config_file.json

## 	Solution Demo:


https://github.com/YasmineElegily/Car_Platform_Cls_LLM_LangChain/assets/69461886/3154cda1-aa20-4bb0-b7c8-f41f6ba54134


*Note: Write at least 1 digit after pasting the car description to Gradio's textbox.*
