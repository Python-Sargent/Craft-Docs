## Api

Everything that is not written in C and CPP uses Python. (besides CMake and GLSL)

### builder.py

#### Block Types

```py
EMPTY = 0          # 'Air'
GRASS = 1          # normal 'grassblock'
SAND = 2           # sand (falling node)
STONE = 3          # stone
BRICK = 4          # clay brick
WOOD = 5           # original wood
CEMENT = 6         # cement
DIRT = 7           # dirt 
PLANK = 8          # planks
SNOW = 9           # snow grassblock
GLASS = 10         # clear glassblock
COBBLE = 11        # cobblestone
LIGHT_STONE = 12   # light textured stone
DARK_STONE = 13    # dark textured stone
CHEST = 14         # chest
LEAVES = 15        # leaves uses transparency
CLOUD = 16         # cloud block unwalkable
TALL_GRASS = 17    # grass plant
YELLOW_FLOWER = 18 # dandelion
RED_FLOWER = 19    # poppy
PURPLE_FLOWER = 20 # tulip (not sure why it's purple)
SUN_FLOWER = 21    # sunflower
WHITE_FLOWER = 22  # orchid
BLUE_FLOWER = 23   # grape hyacinth
```

#### Functions

`sphere()` function:

```py
sphere(cx, cy, cz, r, fill=False, fx=False, fy=False, fz=False)
```

Make a sphere at position `cx, cy, cz`. Filled if `fill` is true. `fx, fy, fz` (undocumented).

---

`circle_x()`

```py
circle_x(x, y, z, r, fill=False)
```

Makes a circle with the center point a `x, y, z`, and a radius of `r`, facing along the x axis. Filled if `fill` is true.

---

`circle_y()`

```py
circle_y(x, y, z, r, fill=False)
```

Makes a circle with the center point a `x, y, z`, and a radius of `r`, facing along the y axis. Filled if `fill` is true.

---

`circle_z()`

```py
circle_z(x, y, z, r, fill=False)
```

Makes a circle with the center point a `x, y, z`, and a radius of `r`, facing along the z axis. Filled if `fill` is true.

---

`cylinder_x()`

```py
cylinder_x(x1, x2, y, z, r, fill=False)
```

Make a cylinder from point `x1` to point `x2` with `y` and `z` giving the other axes of the positional argument, with a radius of `r`.
Filled if `fill` is true.
ving the y and x of the two points `x1` and `x2`
---

`cylinder_y()`

```py
cylinder_y(x, y1, y2, z, r, fill=False)
```

Make a cylinder from point `y1` to point `y2` with `x` and `z` giving the other axes of the positional argument, with a radius of `r`.
Filled if `fill` is true.

---

`cylinder_z()`

```py
cylinder_z(x, y, z1, z2, r, fill=False)
```

Make a cylinder from point `z1` to point `z2` with `x` and `y` giving the other axes of the positional argument, with a radius of `r`.
Filled if `fill` is true.

### world.py

Simple script that helps with the python side of world making.

### server.py

Runs Multiplayer server scripts.

Makes server/client objects/functions.

#### Packet Codes

```py
AUTHENTICATE = 'A'
BLOCK = 'B'
CHUNK = 'C'
DISCONNECT = 'D'
KEY = 'K'
LIGHT = 'L'
NICK = 'N'
POSITION = 'P'
REDRAW = 'R'
SIGN = 'S'
TALK = 'T'
TIME = 'E'
VERSION = 'V'
YOU = 'U'
```