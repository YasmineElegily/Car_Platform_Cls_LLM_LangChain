# Car_Platform_Cls_LLM_LangChain
Improving our online car-selling platform by allowing users to add cars with images, text descriptions, and prices for a more convenient selling experience. 

This is the link to the data: "https://drive.google.com/file/d/1gibdLQwr8JkgTy2ek_pvK3_xF6ZbytaE/view?usp=sharing"

After observing the data and reading the data_info.txt file about it I noticed very small classes like 'Van', 'Wagon' & 'Minivan'.
So I decided to do:
1) Data Augmentation
2) Weighting Classes in the model training
3) Fine-Tuning a Pre-trained Model
4) Drop-out and Kernel Regularization to decrease overfitting
*More approaches I tried to mitigate huge data imbalance*:
5) Try the Focal Loss Function
6) Try LearningRateScheduler
7) Ensemble modeling
8) Re-weighting Classes
9) Resample the lowest classes on Roboflow.
(I did resample the 3 lowest classes on Roboflow but still did not reach optimal results. Training pre-trained models on larger data takes time.)

This is the link to the resampled data: "https://drive.google.com/file/d/1-xcNvK21bjEHE087EgpvntJ2BYd7UnJR/view?usp=drive_link"

# Instructions
To run the LLM and LangChain Test, You need to make a config_file.json for the sensitive data to not be exposed.
Mine's structure for example:

{
	"OPENAI_API_TYPE": "your_api_type",

	"OPENAI_API_VERSION": "your_api_version",

	"OPENAI_API_BASE": "your_api_base",

	"OPENAI_API_KEY": "your_api_key",

	"engine": "you_engine",

	"SenderEmail": "your_email@gmail.com",

	"SenderPassword": "************",

	"RecepientEmail": "recepient.email",

	"ZapierApiKey": "your_zapier_api_key"
}
