Good day to you!

Thanks for visiting my repo.

I've created this during my week off on vacation. I've never really dabbled much into machine learning but the bug bit me and now I'm all in.

The system I've designed in the IPYNB thats listed will dynamically create tensors and plug it into the training loop. It also has optimization systems to ensure that smaller tensors have different learning rates compared to bigger ones (Bigger meaning more batch availability).
It uses yFinance to create the tensors and has auto retry mechanisms effectively automating the entire process. It will allow you to create a dataset via the modification of the methods creating the dataframe for the tensor. 

This system can be applied to any model. If you choose to modify it please target the dataFrame structuring process and the training loop is pretty well designed and integrated with tensorboard.

My model is mainly for processing financial information. It's pretty simple and I'm still in progress training it at this time (2024-01-07) 

I hope my tools can help you in your journey in machine learning and financial analysis, Good Luck!
