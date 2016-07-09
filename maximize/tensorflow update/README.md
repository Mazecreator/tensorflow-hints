# Integrate "optimizer.maximize()" into *TensorFlow*

If you have the development version of Tensorflow installed and wish to integrate the
maximize() function within the tool, you can update the "\\tensorflow\tensorflow\python\training\optimizer.py"
with the content of the "optimizer.py" file.  This update was done on the **R0.9.0 code**.  If
you are updating a later (or earlier) version, you will likely only want to cut-n-paste the
"maximize()" function into your local copy of "optimizer.py".

**Be sure to recompile your TensorFlow repository after the file update.**
