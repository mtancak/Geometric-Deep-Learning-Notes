# Geometric-Deep-Learning-Notes
Notes and Review of the Geometric Deep Learning Proto-book by M Bronstein, J Bruna, T Cohen and P Velickovic

https://arxiv.org/abs/2104.13478

https://www.youtube.com/watch?v=PtA0lg_e5nA&list=PLn2-dEmQeTfQ8YVuHBOvAhUlnIPYxkeu3

## To-Do
* Remove incomplete sections
* Add notes for the remaining parts of the book and lectures
* Clarify some points in the notes
* Practice applying the theory

## Introduction
These are my notes for the Geometric Deep Learning proto-book by Michael M. Bronstein, Joan Bruna, Taco Cohen and Petar Veličković, as well as their youtube AMMI course. These notes cover around the first half of the book and the first 6 lectures of the course. The main reason for these notes is to cover some of the prerequisite knowledge and cover the main points covered in the material. Most of the material in these notes is not my own, it is mostly a collection of images and quotes/rewordings from different sources.

## Thoughts
I think this book is interesting and important because it lays out the groundwork for explaining the structure (symmetries) in different data domains, which can be used to reason about and derive the different architectures used in deep learning. Even though this idea is iterated several times in the presentation of the content, after reading the book I came to the same conclusion and resonated with that idea the most. Recently working with classical computer vision problems that span many different data modalities in medicine, I struggled to reason about the intuitions I had about the structure and symmetries in the data that could be exploited with deep neural networks. This is particularly because as a novice, I followed the most explored, most popular flavour of computer vision, tackling 2D images, which is a box that is too small for many problems I solve to fit in.

One of the problems that I am interested in the most is medical registration of two similar surfaces, such as joints between a pair of bones. Reading the book and following the course gave me a lot of inspiration on how to express the intuitions I have about how these problems should be tackled. By expressing these intuitions as symmetries, one can begin to think about potential architectures in terms of building blocks of invariant and equivariant functions which exploit the symmetries that describe the mechanics that our brain understands in such problems. Conveniently, we can combine these architecture building blocks to create more complex structures in a similar way to combining intuitions about a problem. For example, we can represent intuitions about the mechanics of the movement in joints in terms of symmetries in the domain which expresses the system. These building blocks can then be combined and built-upon to express how information has to be passed. Then, if we think that some problem fits a graph, we can express more complex intuitions in terms of how they fit a certain way of moving the data around the network, which parameters in a network may be related, and so on. 

As the book isn’t restricted to a single domain but instead tries to cover as large a range of domains as possible, these ideas can be transferred over between them. This means you can think of the same problem, with similar building blocks, in terms of different domains which lend themselves to different devices that can be used to model intuitions. This idea gave me the opportunity to do the opposite of representing intuitions in AI architectures - to approach problems from the perspective of different architectures / domains, allowing me to spot new intuitions to try to explore. 
