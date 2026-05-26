# ComfyUI Video Workflows

This repository contains a curated collection of ComfyUI workflows for video generation, video editing, video outpainting, object removal, and video upscaling. The workflows are provided as `.json` files and can be imported directly into a ComfyUI environment, enabling users to test, adapt, and extend the pipelines for their own creative, professional, or research applications.

The repository is organised into three main folders:

- `workflows/`  
  Contains the ComfyUI workflow files in `.json` format. These files can be imported directly into ComfyUI and used as ready-made pipelines for a range of video-related tasks.

- `ComfyUI screenshots/`  
  Contains screenshots of each workflow as displayed in the ComfyUI interface. These images provide a quick visual reference for the node layout, structure, and logic of each workflow.

- `examples/`  
  Contains example outputs generated using the workflows. These examples illustrate the intended use cases and visual capabilities of each pipeline.

## Workflows

### Remove Object from Video - LTX 2.3 LoRA

This workflow is designed for removing unwanted objects from the foreground of a video clip. Users upload an input video and provide a prompt describing the object that should be removed, allowing the workflow to perform targeted video editing while preserving the overall continuity of the clip. It is useful for scene clean-up, compositional refinement, and post-production adjustments where distracting elements need to be erased. The workflow provides a practical solution for prompt-guided video object removal in ComfyUI.



https://github.com/user-attachments/assets/81cad117-afed-483a-9b87-93055f66b540



### Seedance 2.0 for Advertising Workflow

This workflow is intended for creating polished advertising-style B-roll content. It supports three main approaches: prompt-only video generation, reference-guided generation using one or more images, and light video editing for enhancing or replacing short clip segments. This makes it suitable for product visualisation, branded inserts, promotional content, and short cinematic shots for advertising applications. Its structure gives users flexible control over style, object identity, timing, and visual continuity.



https://github.com/user-attachments/assets/20d29e53-a90b-4b74-82a2-57890b2df26f



### Video Outpainting - LTX 2.3 Video LoRA

This workflow performs video outpainting by expanding the canvas of existing footage and synthesising new visual content beyond the original frame boundaries. It is especially useful when converting footage into a new aspect ratio, extending backgrounds, adding extra visual space for reframing, or adapting clips for different screen formats. The workflow is designed to preserve the original content while generating coherent surrounding imagery that remains visually consistent across frames. It is therefore well suited to both creative expansion and practical post-production tasks.

<img width="296" height="258" alt="Video Outpainting  LTX 2 3 Video LoRA (2)" src="https://github.com/user-attachments/assets/c86db260-52d3-4682-9598-099eceb0ea31" />


### Video Upscale - Topaz Starlight Precise 2.5

This workflow is designed to enhance video resolution using the Topaz Starlight Precise 2.5 model. Its primary function is to upscale video content to sharper, cleaner high-resolution output, with a particular emphasis on improved detail and reduced visual artifacts. It is suitable for restoring or enhancing lower-resolution footage, preparing content for 4K delivery, and improving overall video fidelity in professional production pipelines. The workflow offers a streamlined ComfyUI-based approach to AI-assisted video enhancement.



https://github.com/user-attachments/assets/96e4f4d9-8696-4842-a1f3-9246e3967382



## How to Use

1. Open ComfyUI.
2. Drag and drop a `.json` file from the `workflows/` folder into the ComfyUI canvas, or load it through the ComfyUI interface.
3. Check that all required models, custom nodes, and dependencies are installed in your local ComfyUI environment.
4. Add or replace the input videos, reference images, and prompts where required.
5. Queue the workflow and review the generated output.
6. Compare your results with the files in the `examples/` folder where relevant.

## Notes

Some workflows may require specific models, custom nodes, or hardware resources to run successfully. If a workflow does not execute immediately, check the missing-node or missing-model messages in ComfyUI and install the necessary components before retrying.

The workflows in this repository are intended as practical starting points. Users are encouraged to adapt prompts, frame settings, seeds, model parameters, and node structures according to their own creative, technical, or research requirements.

## Acknowledgements

The workflows in this repository are based on publicly available ComfyUI workflow examples and model ecosystems, including workflows documented on Comfy.org. Please consult the relevant workflow pages, model documentation, and licensing terms for each workflow and associated model before using them in production, commercial, or research contexts.

## Repository Structure

```text
ComfyUI-vid-workflows/
│
├── workflows/
│   ├── Remove Object from Video - LTX 2.3_LoRA.json
│   ├── Seedance 2.0 for Advertising Workflow.json
│   ├── Video Outpainting - LTX 2.3 Video LoRA.json
│   └── Video Upscale_Topaz Starlight Precise 2.5.json
│
├── ComfyUI screenshots/
│   └── Screenshots of each workflow in ComfyUI
│
└── examples/
    └── Example outputs generated using the workflows
