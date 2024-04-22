# Autoencoders_FashionNumbers
ABSTRACT: Autoencoders: Generating Fashion &amp; Numbers from MNIST datasets

- Loads MNIST fashion and digits dataset
- Stacked, Convolutional, and Recurrent Autoencoders to generate images from the partial, original fashion/digits images

## Discussion

What is an autoencoder?
-> An autoencoder is an articial neural network
  - Used with unsupervised learning
  - Learns efficient representations of input data
    - Uses dimention reduction
(ChatGPT helped me learn)
  - Compiles the encoder and decoder to create a history and codings output

- Here, the first row of images is the origional, and the second row is the reconstructions

### Stacked Autoencoder
- More neurons, more layers
- Use with fraud detection

### Convolutional Autoencoder
- Like a puzzle, looks at small parts of puzzle to understand larger picture
- Use with facial recognition

### Recurrent Autoencoder
- Can process time-series data, data with differing lengths
- Used for text generation, speech recognition
- Representing sequential data (ChatGPT helped)


-------




1. Discuss how effective was auto encoders in generating images:
  - In the fashion dataset, the stacked, convolutional, and recurrent autoencoder results are indistiguishable, but the 'original' data is changed slightly
    - I'd say the convolutional autocoder did best with this data; the images produced seem to be the most detailed and close to the originals.
  - In the digits dataset, again it seems like the bottom row of data changes slightly, but the top row remains practically the same.
    - I would say the recurrent autoencoder did best, since the numbers produced are the most clear

2. Discuss how you can improve the architecture for better image generation:
  - I think the main thing is to choose the appropriate autoencoder for each task.
  - For image generation, it depends on what you want to generate
    - It makes sense that the convolutional autoencoder does best with the fashion dataset, since the convolutional model looks at small parts of the image and learns to apply it to the big picture
    - For the digit dataset, I would think the convolutional would also work better, but maybe because the recurrent is used more with numbers, it works better?
      - We could try more layers, more neurons, but we don't want to overfit the data, so it would depend on what the outputs do.

**References**: Géron, A. (2023). Hands-on machine learning with scikit-learn, Keras, and tensorflow: Concepts, tools, and techniques to build Intelligent Systems. O’Reilly Media. 
