# FoodClassifier

The project based on food will classify the users pick of image using image classification such as imagenet and models such as resnet18.

![Picture](file:///C:/Users/dleer/OneDrive/Desktop/hamburger1.jpg)

## How it is developed

The project uses the model resnet18 with datasets of multiple food families. When the program is being run, it will use imagenet to classify the correct image and the name of the food


## How to run the program

1. Make sure you have correct dataset
2. Get labels.txt and resenet18 model
3. Run the docket container
4. To train images, use model-dir, python3 train.py --model-dir=models/"name of dataset" data/"name of dataset"
5. Run onnx export script
6. Run imagenet.py --model=$NET/resnet18.onnx --input_blob=input_0 --output_blob=output_0 --labels=$DATASET/labels.txt $DATASET/test/"name of dataset"/"name of image" "output file"
7. Scp the finished imagenet.py
