---
layout: post
title: ExaDGLM
excerpt_separator:  <!--more-->
---

ExaDGLM updates the original [ExaDGLM](https://jaeminshin-cse.github.io/)
theme for [Jekyll](http://jekyllrb.com) 3.x and 4.x and adds new functionality.

### An Introduction to the Discontinuous Galerkin Method

In the realm of numerical methods for solving partial differential equations (PDEs), the Discontinuous Galerkin (DG) method has gained significant attention over the past few decades. In contrast to traditional finite element methods, which require the solution to be continuous across element interfaces, DG methods allow for solutions to be discontinuous.

### What is the Discontinuous Galerkin Method?

The Discontinuous Galerkin method is a numerical method for solving partial differential equations. It is particularly effective when dealing with problems with solutions that exhibit shock or discontinuity. The main principle behind DG methods is allowing for a piecewise discontinuous representation of the solution across the mesh elements.



### Why use the Discontinuous Galerkin Method?

DG methods are renowned for their flexibility and robustness. Here are some reasons why you might consider using DG methods:

* Flexibility: DG methods can handle complex geometries and adaptive meshes.
* High Order Accuracy: DG methods can achieve high order accuracy with appropriate choice of basis functions.
* Robustness: DG methods can handle solutions with shocks or discontinuities.


### How Does the Discontinuous Galerkin Method Work?

The DG method combines features from both Finite Element and Finite Volume methods. Similar to Finite Element methods, DG methods use a local basis to represent the solution within each element. However, like Finite Volume methods, DG methods apply conservation laws in an integral form.

The primary steps for implementing the DG method include:

* Discretize the Domain: Divide the computational domain into elements.
* Approximate the Solution: Within each element, approximate the solution as a linear combination of basis functions.
* Apply the Weak Form: Multiply the governing PDE by a test function, integrate over each element, and apply integration by parts.
* Enforce Continuity: Apply suitable numerical fluxes at the interfaces between elements to maintain the conservation property.

While the DG method comes with many benefits, one should also be aware of the associated computational cost, which can be high due to the increased number of degrees of freedom. Furthermore, the choice of numerical flux is crucial for the stability and accuracy of the method.

### Closing Thoughts

The Discontinuous Galerkin method provides a robust and flexible approach to solving PDEs, especially when dealing with problems that involve shocks or discontinuities. Its unique features allow it to handle complex geometries and adaptive meshes with high order accuracy, making it a popular choice for a variety of applications in science and engineering.

However, like any numerical method, the DG method comes with its own set of challenges, including higher computational cost and the careful selection of numerical fluxes. As always, the suitability of the DG method depends largely on the specific problem at hand.
