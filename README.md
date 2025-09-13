# ComfyUI_ForLoop
Simple workflow showing how to use the For Loop nodes in ComfyUI.

It uses two values, an integer for value1, and a string for value2.

The integer is incremented by one on each iteration, and concatenated to the string with a separator.

The two values are output at the end.

## Main concepts to grasp

* Use the flow ports to link the start and end nodes, this enables the flow of control between them.

* Each value is initialised at the input of the start node, and is served at the output of the start node to be consumed at each iteration

* Once the processing is done in the "body" (between the start and end node) the updated data for that value would be fed into the initialisation port of the end node

* the flow of control between the two nodes will ensure the transfer of the updated data in the next loop iteration.

## Custom node packages used in this workflow

* **[ComfyUI-Easy-Use](https://github.com/yolain/ComfyUI-Easy-Use)**: A comprehensive node package that simplifies and enhances many common ComfyUI tasks.
* **[ComfyUI-Various](https://github.com/jamesWalker55/comfyui-various)**: A collection of various utility nodes for image, primitive, and color operations.

Ensure these are installed in your `ComfyUI/custom_nodes` directory for the workflow to function correctly.
Or use the **[ComfyUI-Manager]( https://github.com/Comfy-Org/ComfyUI-Manager)** to install them.
