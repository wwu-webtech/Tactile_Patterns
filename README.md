## What is this?:
A barebones version of the python backend for testing on azure using a python webapp. Contains an existing folder of images that can be used by running `python -c "from function_app import process_img;process_img('test_photos/{image.jpg}')"`. This will result in the processed images being in the /tmp directory.

## Installation:

1. Start by installing python, which can be found [here](https://www.python.org/downloads/) or by running `sudo apt install python`. 
2. Run `git clone https://github.com/velo1guy/tactile_patterns_web.git`.
3. Enter this directory, and in the `azure_tactile` subdirectory, run `python -m venv venv` and your virtual enviornment should be set up.
4. Once in the venv, run `pip install -r requirements.txt`, and your requirments should be installed. 

## Next Steps:

Next steps here will be to make sure this works on azure and then sending it post requests, which it should be set up for already.


