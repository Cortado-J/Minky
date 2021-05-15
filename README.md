# Minky

Exploration of Adding images using Minkowski Sum

Minkowski Sums are fairly resource hungry...
For a Minkowski sum of two n x n images, the output is 2n x 2n pixels.
For each pixel we need to make "up to" n x n = n^2 calculations.
So total of "up to" 4n^4 calculations in total.
So for two 100 x 100 images we need "up to" 400,000,000 operations!

"Up to" because it's actually less than the above calculations show as many
pixels depend on fewer input pixels.
The Order is about right but need to do some maths to work out the number.

So we use GPU.JS which gives us access to the GPU's parallel capabilities.
https://gpu.rocks/#/
