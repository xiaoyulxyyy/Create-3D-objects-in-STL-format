# Create-3D-objects-in-STL-format

The objective of this project is to convert a 2D image to a 3D object for 3D printing.
There are a few things that need to be understood in order to proceed.

1. Understand the file format that is used for Stratasys J750
2. Understand RGB 
3. What does it mean by 2D-->3D?Lack of depth/height data? 

The answer to the questions above:
1. Software used by Stratasys is GrabCAD Print. GrabCAD Print supports STL and VRML files. Therefore, next step is to understand what is STL and how is it coded.

**What is STL?**
- It is a file format native to stereolithography CAD software
- It describe only the surface grometry of a three-dimensional object without any representation of colour, texture or other common CAD model attributes.
- STL format specifies both ASCII and binary representations
- Binary files are more common
- Binary files are compact
- It describes raw, unstructured triangulated surface by the unit normal and vertices of the triangles using three-dimensional Cartesian coordinate system.
- It contain no scale information, the units are arbitrary

Since we have understood that STL describes only the surface geometry of 3D object, and a 3D object is formed by vertices and faces. Therefore, find out more about mesh modelling. 

**What is a mesh in 3D modelling?**
- 3D models are modelled out of polygons that are connected at their edges and vertices to define the shape of an object in 3D. Therefore, a collection of polygons is called a mesh

![image](https://user-images.githubusercontent.com/88549766/133472634-576cebc0-3db5-48aa-8399-4230dae27782.png)

With the information above, we can proceed with coding the 3D object in STL format. 
