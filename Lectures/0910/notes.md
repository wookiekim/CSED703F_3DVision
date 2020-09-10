# 200910

## Term Project
60% of the credits
* Co-evaluated by other students
* Peer review
* Penalty once the topic is not really related to 3D vision

One/Two students per team
* Higher level of expectation for a two-person team

Show-case video required

## Multiview Geometry
Using multiple views to obtain geometry
* 3D reconstruction
#### Course Objective
1. connect the dots between 3D scenes and 2D images
* pinhole camera model
* camera pose estimation
  * analogous to 3D reconstruction (tightly coupled problem)

2. Learn how to recover 3D scene
* Image rectification
* Stereo matching (aka 2-view geometry)

3. Learn what modern approaches are trying to achieve
* Correpondences from geometric configuration
  * could be used for semisupervision
* can recover 3D scene from ill-posed configuration?
  * an open question
  * from a single view?

Textbook: Multiple view Geometry in computer vision
* Richard Hartley and Andrew Zisserman
* Nothing on deep learning, very mathematic

In terms of accuracy:
* Single view < Stereo < Multiview
* analogous to "increasing # equations" in simultaneous equations

Google Research: Learning depths of Moving people by watching frozen(CVPR 2019)
* UNet: mentioned a lot, a must-read 
* MannequnChallege Dataset (TPAMI 2020)
* Loss at valid MVS pixels (partially annotated)

Preliminary Mathematics : Mostly Linear Algebra
* Homogeneous coordinates
  * overall scaling is not important
     * so long as the scaling factor is not 0 
  * useful in projective geometry for:
    * basic repr of geometric entities (points, lines, planes)
    * transformations
    * repr of point and line at inf

* Cross product
  * magnitude == area of parallelogram with the vectors for sides
  * != vector product (inner product, normalized)

* Lines, Points, their relations in 3D
* Representing translation/rotation/similarity/affine...etc in the form of linear algebraic expressions
* Projective transform is the key in 2D <> 3D
* All well summarized in ppt

Q. Why is projection 8dof instead of 9?
* The scaling factor is not considered independent (homogeneous characteristic)
* [More details here](https://link.springer.com/content/pdf/bbm%3A978-0-85729-046-5%2F1.pdf)

Pinhole camera: perspective projection
* orthographic projection is difficult to see in practice
  * a special case of perspective projection


