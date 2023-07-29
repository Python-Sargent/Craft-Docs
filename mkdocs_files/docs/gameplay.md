## Controls

- WASD to move forward, left, backward, right.
- Space to jump.
- Left Click to destroy a block.
- Right Click or Cmd + Left Click to create a block.
- Ctrl + Right Click to toggle a block as a light source.
- 1-9 to select the block type to create.
- E to cycle through the block types.
- Tab to toggle between walking and flying.
- ZXCVBN to move in exact directions along the XYZ axes.
- Z to zoom.
- F to show the scene in orthographic mode.
- O to observe players in the main view.
- P to observe players in the picture-in-picture view.
- T to type text into chat.
- Forward slash (/) to enter a command.
- Backquote (`) to write text on any block (signs).
- Arrow keys emulate mouse movement.
- Enter emulates mouse click.

---

## Chat Commands

```
/goto [NAME]
```

Teleport to another user.
If NAME is unspecified, a random user is chosen.

```
/list
```

Display a list of connected users.

```
/login NAME
```

Switch to another registered username.
The login server will be re-contacted. The username is case-sensitive.

```
/logout
```

Unauthenticate and become a guest user.
Automatic logins will not occur again until the `/login` command is re-issued.

```
/offline [FILE]
```

Switch to offline mode.
FILE specifies the save file to use and defaults to "craft".

```
/online HOST [PORT]
```

Connect to the specified server.

```
/pq P Q
```

Teleport to the specified chunk.

```
/spawn
```

Teleport back to the spawn point.

---

## Multiplayer

In multiplayer mode, players can observe one another in the main view or in a picture-in-picture view.
Implementation of the PnP was surprisingly simple - just change the viewport and render the scene again from the other player’s point of view.

---