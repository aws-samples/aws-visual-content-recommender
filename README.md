## Visual content recommender

This repository guides users through creating a visual content recommender/search to search similar images using Amazon SageMaker and Amazon Elasticsearch

## How does it work?

Each reference image from Caltech101 dataset is represented as a 2048 feature vector using a convolutional neural networks and gets stored into Amazon Elasticsearch KNN index

![diagram](../master/pic1.png)

When we present a new query image, it's computing the related feature vector from Amazon SageMaker hosted model and query Amazon Elasticsearch KNN index to find similar images

![diagram](../master/pic2.png)

## License

This library is licensed under the MIT-0 License. See the LICENSE file.
