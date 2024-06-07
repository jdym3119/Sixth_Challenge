# Sixth_Challenge
In this challenge we have to take the code of the [last challenge](https://github.com/jdym3119/Fifth_Challenge), Shapes and making exceptions on it and also, making exceptions in the code of the [first_repository](https://github.com/jdym3119/First_Challenge) that we made for OOP class:

## First_repository

I added the commonly exceptions like `ValueError` - `ZeroDivisionError` - `TypeError`
## Shape

We add some exceptions in this package, the new exceptions made:


1. The user can't enter strings in the program where it doesn't correspond


2. We created an own exception that appers when the user add more than two times the same vertex, this stop the program 
and don't let the program create the object

```python
different_vertices = []

      for vertices_comparer in vertices:
        if vertices_comparer not in different_vertices or different_vertices == []:
          different_vertices.append(vertices_comparer)        

      if len(different_vertices) != len(vertices):
        raise UserError(f"Vertices are not unique {vertices}")
```


