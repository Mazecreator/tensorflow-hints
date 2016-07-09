# Maximize a function in TensorFlow
## Implementation is also known as Gradient Ascent
To maximize a function in TensorFlow: **Minimize(-FunctionValue)**

How to maximize may be obvious to most users of TensorFlow, but it was not to me.  Given the automatic gradient calculation, I was not certain this would work since the gradient was calculated from the "cost" function as passed to "minimize(cost)".

Also, this does not make the code very readable, easy to use, or user friendly as you would write to maximize a "**value= Max(F(x))**":

>**max_op = tf.train.GradientDescentOptimizer(0.01).minimize(-value)**

I have a few options in this section of the hints.

You can simple add a small python function to your code as offered by one of the contributors [girving](https://github.com/girving):

    def maximize(optimizer, value, ...):
      return optimizer.minimize(-value, ...)


If you have the developer version of TensorFlow on your system, you can add the "maximize()" function to your distribution.  Please see the "tensorflow update" folder for the "optimizer.py" and "README.md" file with instructions.

Once you install one of these two code segments, you will be able to change the python script to read better:

>**max_op = tf.train.GradientDescentOptimizer(0.01).maximize(value)**

I have enclosed a Notebook file to prove that maximization works.