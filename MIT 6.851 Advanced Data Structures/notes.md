# MIT 6.851 Advanced Data Structures, Spring 2012
Instructor: Erik Demaine

Link:
https://www.youtube.com/playlist?list=PLUl4u3cNGP61hsJNdULdudlRL493b-XZf

## 3. Geometric structures I.

### Planar point location
- points on 2d space, and edges between them. no crossing edge -> partition of space
- STATIC version: given (could be preprocessed because it's static) map, which face contains point (x,y)
- DYNAMIC: insert/delete edges

- SWEEPING LINE ALGORITHM: We have segments on a plane, which are intersecting? Let's use a sweeping vertical line, starting from min(x), points ordered by x.
  Try to keep the current y order of the segments in a queue. If the next point is a start, insert by y. If the order changed since the previous points, there was an intersection.
  https://youtu.be/NMxLL3D5qd8?si=1ewSSl0yPhRCmc9Y&t=391
- this cross section DS is usually a BBST (balanced binary search tree) 

  
