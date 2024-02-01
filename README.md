## sd-ratio-lock-plus

An extension for [AUTOMATIC1111/stable-diffusion-webui](https://github.com/AUTOMATIC1111/stable-diffusion-webui) that deals with aspect ratios. 
* can lock image height to width. Change height and width will change to match it, so that aspect ratio is maintained.
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

## Use

Select an option from the Image Ratio dropdown. This will lock the height slider to the width slider. To unlock the sliders select None from the dropdown. Select the magnifying glass to attempt to identify the Ratio based on the current width and heights.

NOTICE: Currently the way that gradio callbacks work this only works when the width changes. Also since this is a client to server to client solution the order of operations sometimes gets missed. (i.e. It requires you to jiggle the width slider to get the correct height)

## Roadmap

- add option to keep the exact aspect ratio of image
- Allow for custom ratios

## Credit
bit9labs