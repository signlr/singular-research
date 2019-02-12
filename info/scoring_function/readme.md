# Scoring function

The scoring function accepts our data as an input and maps the data to class labels. For instance, given our set of input images, the scoring function takes these data points, applies some function f (our scoring function), and then returns the predicted class labels, similar to the pseudocode below:

```INPUT_IMAGES => F(INPUT_IMAGES) => OUTPUT_CLASS_LABELS```

`sF = W * Xi + b`

## Weight

Our weight matrix W contains three rows (one for each class label) and 3,072 columns (one for each of the pixels in the image)

`x_flatten = (img_w) * (img_h) * (img_depth)`

Assuming we have an image 32x32x3 (3 depth RGB)
`x_flatten = 32 * 32 * 3 = 3072`

`W = (#class labels) * (x_flatten)`
