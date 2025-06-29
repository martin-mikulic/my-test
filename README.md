## My Test: Unity WebGL vs Native Spine Player

I recently tested the file size and performance differences between Unity WebGL and the native Spine player for a simple Spine animation project.

👉 **Unity WebGL Version:**
[Live Demo](https://martin-mikulic.github.io/Spine_Zagor/)

* **Total Size:** \~23 MB

  * **Assets:** \~13 MB
  * **Engine & Build Files:** \~10 MB

👉 **Native Spine Player:**
[Live Demo](https://martin-mikulic.github.io/my-test/) *(loads much faster)*

* **Total Size with PNG Assets:** \~13 MB
* **Total Size with JPEG Assets:** \~2.5 MB *(impressively small but no transparency)*
* **Player Size:** \~0.5 MB

The loading time difference is huge—using JPEGs makes it practically instant. Unfortunately, I need PNG transparency, but even then, the native player cuts the size nearly in half compared to WebGL.

Overall, it's great to see how efficient the native Spine player can be for lightweight deployments!

Spine itself only allows exporting all images in one format, but in Unity you could selectively convert non-transparent images to JPEGs to save space. This can be a viable technique if your workflow supports it.
