## What is this?:

This is a python backend made for testing on the tactile images project's capabilities to be deployed as an Azure python web app. It contains an existing folder of images that can be used by entering the virtual environmentt, then running `python3 -c "from __init__ import process_img;process_img('test_photos/{image.jpg}')"`. This will result in the processed images being in the /tmp directory.

## Local Installation:

1. Start by installing python, which can be found [here](https://www.python.org/downloads/), or by running `sudo apt install python`.
2. Run `git clone https://github.com/velo1guy/tactile_patterns_web.git`.
3. Enter this directory, and in the `azure_tactile` subdirectory, run `python -m venv venv` and your virtual environment should be set up.
4. Once in the venv, run `pip install -r requirements.txt`, and your requirements should be installed.
5. Run `python3 -c "from __init__ import process_img;process_img('test_photos/{image.jpg}')"`, and the selected image should be processed, with the new tactile_image located in the processed_images directory.

## Remote Deployment Installation:

This section is currently still under construction, while it works, images are saved to the tmp directory, which is not public and therefore inaccessible for this projects uses.

1. Go to the [Azure portal](https://portal.azure.com/#home).
2. Click on "Create a Resource" > "Create a Function App".
3. Enter your information, with the python Runtime Stack.
4. Select the different settings as desired, selecting this repository as the deployment source.
5. Create the function and click on it on the home page.
6. The function should automatically boot up. You can then go into "Developement Tools" > "SSH" to get to the terminal.
7. Run `python3 -c "from __init__ import process_img;process_img('test_photos/{image.jpg}')"`, and the selected image should be processed, with the new tactile_image located in the processed_images directory.

## Next Steps:

Next steps here will be to make a module saving the images to a blob storage container so that processed images can be viewed.
