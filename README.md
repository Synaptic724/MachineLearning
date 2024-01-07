Good day to you!

Thanks for visiting my repo.

I've created this during my week off on vacation. I've never really dabbled much into machine learning but the bug bit me and now I'm all in.

The system I've designed in the IPYNB thats listed will dynamically create tensors and plug it into the training loop. It also has optimization systems to ensure that smaller tensors have different learning rates compared to bigger ones (Bigger meaning more batch availability).
It uses yFinance to create the tensors and has auto retry mechanisms effectively automating the entire process. It will allow you to create a dataset via the modification of the methods creating the dataframe for the tensor. 

This system can be applied to any model. If you choose to modify it please target the dataFrame structuring process and the training loop is pretty well designed and integrated with tensorboard. You will also need to download the listing_status, and the progress_tracker.csv and modify the directories the classes that use them are targetting. There is a decent amount of data that you can play with from yFinance. Currently it takes a tensor from the progress_tracker list and modifies it with VIX and adds a few indicators then generated a combined dataset that goes into the model. After each iteration of epochs it generates a new tensor and modifies the learning rate, batch size depending on batch count in each tensor.

There is also optuna built into the system. You will need to modify the tensor input because it will still randomize the tensor so to generate a new tensor of similar size just modify the progress tracker with the same ticker to give you the best optimization because you will want to test your model on the same tensor and to give you a good result. I used 10 epochs it was pretty good. 

My model is mainly for processing financial information. It's pretty simple and I'm still in progress training it at this time (2024-01-07) 

I hope my tools can help you in your journey in machine learning and financial analysis, Good Luck!
