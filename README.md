## sd-ratio-lock-plus

An extension for [AUTOMATIC1111/stable-diffusion-webui](https://github.com/AUTOMATIC1111/stable-diffusion-webui) that deals with aspect ratios. 
* can lock image height to width. Change width, and the height will change to match it, so that aspect ratio is maintained.
* can snap your image to the closest useful aspect ratio. (i.e. 4:3, 16:9, 1:1, etc.)

#### img2img View
![Ratio Lock](./screenshots/screenshot.png?raw=true "Ratio Lock")

## Installation

The extension can be installed directly from within the **Extensions** tab within the Webui. 
"Install from URL" and paste in the git repo: https://github.com/ima18h/sd-ratio-lock-plus

Manual install from within the webui directory:

	git clone https://github.com/ima18h/sd-ratio-lock-plus

must be inside extensions folder, and then restart your stable-diffusion-webui. 
The lock ratio dropdown will appear under the width and height sliders.

## How to use

Select an option from the Image Ratio dropdown. This will make it so pressing up/down on width, will change height accordingly. 
If you do a big change in width by dragging the slider, then you might have to press up/down to make the height update correctly. 
Changing the height will not change anything, even when an aspect ratio is selected. 
To unlock the sliders select None from the dropdown. 
Select the magnifying glass to identify the Ratio based on the current width and heights. It will always select the closest useful aspect ratio.

## TODO / Roadmap

- add option to keep the exact aspect ratio of image
- Allow for custom ratios

## Credit
bit9labs